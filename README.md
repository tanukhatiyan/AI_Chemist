**AI Chemist App**
_________________________________________________________________________________________________________________________________________________________

AI Chemist is a cutting-edge mobile application designed to provide personalized chemical solutions and experimental recommendations. Built on the advanced Gemini Pro model, AI Chemist leverages artificial intelligence to analyze user inputs, laboratory conditions, and research objectives, delivering tailored experiment designs, chemical synthesis pathways, and insightful data analysis. Its core mission is to enhance research efficiency and innovation in the field of chemistry through intelligent, data-driven guidance.
_______________________________________________________________________________________________________________________________________________________________
*Features*

1.**Streamlit UI**

An intuitive dashboard for inputting data and receiving real-time experiment recommendations.
Dynamic data visualizations for easier interpretation.
Export options for results in PDF or CSV formats, simplifying documentation.

2.**Secure Configuration (dotenv)**

Protect sensitive information, such as API keys and credentials, with dotenv for secure access and environment management.

3.**Google Generative AI Insights**

Experiment Design: AI-generated plans based on lab conditions and goals.
Data Analysis: Automated interpretations and hypothesis suggestions.
Synthesis Pathways: Customizable chemical synthesis routes.
Chat-Based Assistance: Real-time, conversational guidance for experiment support.
______________________________________________________________________________________________________________________________________________________________
*Installation*
_________________________________________________________________________________________________________________________________________________
Clone the Repository

    git clone https://github.com/tanukhatiyan/AI_Chemist
Navigate to the Project Directory
______________________________________________________________________________________________________________________________________________________
Create a Virtual Environment

For Linux/macOS:

    python3 -m venv venv
    source venv/bin/activate

For Windows:

    python -m venv venv
    venv\Scripts\activate
____________________________________________________________________________________________________________________________________________________________
*Install Required Dependencies*


    pip install -r requirement.txt
___________________________________________________________________________________________________________________________________________________________
*Google API Key Setup*

The Google API key authorizes secure access to Google services. It ensures that only authorized users can interact with Google’s resources through the AI Chemist app.

Set Up Google API Key: Visit the Google API Documentation for instructions on generating and configuring your key.
Environment Configuration: Add the key to your .env file for secure management.
Link:https://ai.google.dev/gemini-api/docs/api-key
___________________________________________________________________________________________________________________________________________________________
*Launching the Application*
Start the App

In the terminal, run:

    streamlit run app.py
___________________________________________________________________________________________________________________________________________________________
*Access the App*

Open a browser and go to:


http://localhost:8501
___________________________________________________________________________________________________________________________________________________________
Example Screenshots

![Screenshot 2024-10-27 224301](https://github.com/user-attachments/assets/9a33376d-12b0-4e8b-ac56-02c4944ff68a)
![Screenshot 2024-10-27 224400](https://github.com/user-attachments/assets/545e69ac-7e49-4714-b071-e8d0a1adb801)

