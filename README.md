###AI Chemist App
AI Chemist is a cutting-edge mobile application designed to provide personalized chemical solutions and experimental recommendations. Built on the advanced Gemini Pro model, AI Chemist leverages artificial intelligence to analyze user inputs, laboratory conditions, and research objectives, delivering tailored experiment designs, chemical synthesis pathways, and insightful data analysis. Its core mission is to enhance research efficiency and innovation in the field of chemistry through intelligent, data-driven guidance.

Features
Streamlit UI
An intuitive dashboard for inputting data and receiving real-time experiment recommendations.
Dynamic data visualizations for easier interpretation.
Export options for results in PDF or CSV formats, simplifying documentation.
Secure Configuration (dotenv)
Protect sensitive information, such as API keys and credentials, with dotenv for secure access and environment management.
Google Generative AI Insights
Experiment Design: AI-generated plans based on lab conditions and goals.
Data Analysis: Automated interpretations and hypothesis suggestions.
Synthesis Pathways: Customizable chemical synthesis routes.
Chat-Based Assistance: Real-time, conversational guidance for experiment support.
Installation
Clone the Repository

bash
Copy code
git clone https://github.com/tanukhatiyan/AI_Chemist
Navigate to the Project Directory

bash
Copy code
cd AI_Chemist
Create a Virtual Environment

For Linux/macOS:
bash
Copy code
python3 -m venv venv
source venv/bin/activate
For Windows:
bash
Copy code
python -m venv venv
venv\Scripts\activate
Install Required Dependencies

bash
Copy code
pip install -r requirements.txt
Google API Key Setup
The Google API key authorizes secure access to Google services. It ensures that only authorized users can interact with Google’s resources through the AI Chemist app.

Set Up Google API Key: Visit the Google API Documentation for instructions on generating and configuring your key.
Environment Configuration: Add the key to your .env file for secure management.
Link:https://ai.google.dev/gemini-api/docs/api-key
Launching the Application
Start the App

In the terminal, run:
bash
Copy code
streamlit run app.py
Access the App

Open a browser and go to:

Copy code
http://localhost:8501
Example Screenshots
![Screenshot 2024-10-27 224301](https://github.com/user-attachments/assets/9a33376d-12b0-4e8b-ac56-02c4944ff68a)
![Screenshot 2024-10-27 224400](https://github.com/user-attachments/assets/545e69ac-7e49-4714-b071-e8d0a1adb801)

