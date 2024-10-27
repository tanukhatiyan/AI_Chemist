# AI_Chemist
Pioneering the Future of Chemical Science with Gemini Vision Pro
Install the required libraries
Run the command: pip install -r requirements.txt
Generate Google API Key
Link:https://ai.google.dev/gemini-api/docs/api-key
Interfacing with Pre-trained Model

from dotenv import load_dotenv
load_dotenv()            
import streamlit as st
import os
import google.generativeai as genai
from PIL import Image

genai.configure(api_key=os.getenv("Google_API_KEY"))
def input_image_setup(uploaded_file):
    if uploaded_file is not None:
       bytes_data=uploaded_file.getvalue()
       image_parts =[
           {
               "mime_type": uploaded_file.type,
               "data": bytes_data
           }

       ]
       return image_parts
    else:
       raise FileNotFoundError("No file uploaded")
input_prompt="""

You are an expert pharmacetical/Chemist where you need to see the tablets from the image and, also provide the details of every drug/tablets items with below format

1. Examine the image carefully and identify the tablets depicted.

2. Describe the uses and functionalities of each tablet shown in the image.

3. Provide information on the intended purposes, features, and typical applications of the tablets.
4. If possible, include any notable specifications or distinguishing characteristics of each tablet.
 5. Ensure clarity and conciseness in your descriptions, focusing on key details and distinguishing fa

"""
Model Deployment
We deploy our model using the Streamlit framework, a powerful tool for building and sharing data applications quickly and easily. With Streamlit, we can create interactive web applications that allow users to interact with our models in real-time, providing an intuitive and seamless experience.
st.set_page_config(page_title="AI Chemist App")
st.header("AI Chemist App")
input=st.text_input("Input Prompt:",key="input")
uploaded_file=st.file_uploader("Choose an image...",type=["jpg","jpeg","png"])
image=""
if uploaded_file is not None:
    image=input_image_setup(uploaded_file)
    st.image(uploaded_file,caption="Uploaded Image",use_column_width=True)
submit=st.button("tell me")   
if submit:
    image_data=input_image_setup(uploaded_file)
    response=get_gemini_repsonse(input_prompt,image_data,input)
    st.subheader("The Response is")
    st.write(response)
To host the application,  go to the terminal, type - streamlit run app.py    
