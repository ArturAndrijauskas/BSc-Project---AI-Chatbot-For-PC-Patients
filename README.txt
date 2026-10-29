This project is an AI-powered chatbot designed to provide trustworthy, empathetic, and accessible information about prostate cancer. It aims to support patients, caregivers, and anyone seeking accurate answers about symptoms, diagnosis, treatments, and available support resources. While it does not replace professional medical advice, it serves as a helpful first step toward understanding prostate cancer better.


IMPORTANT ACTIONS:

1. For initial set up, go to Google Colab and "Upload" the finalChatbotProject.ipynb file from the ara38_TechnicalWork_2025 folder

2. You have been provided FAQ data for download within the ara38_TechnicalWork_2025 folder
- This system relies on connection to Google Drive so the download and storage of data.csv is necessary within Drive in the following folder: My Drive/MedBot_Data
- If possible, please connect to Google Drive and ensure this is complete to prevent any possible errors or issues
- An error will be displayed later during general set up after running code Section 2 if data.csv isn't correctly stored

3. This system relies on ngrok, a tool used to create a tunnel between my/your locally hosted web server and an endpoint on ngrok servers, making your local development environment accessible online without needing a public IP or domain name for as long as the application is running.
- Current code displays: !ngrok config add-authtoken 2tiD7xznMIuyWhuOvgetvnnpGBN_8agtxVyhtshgkrBDUPdR6
- This is my personal authentication token used to connect and use ngrok's servers
- After running, if an error is displayed, please navigate and sign in to ngrok's official website where you will be able to copy and paste your own auth token for the servers to be connected and ran with your local device


GENERAL OVERVIEW + SETUP:

The following sections of this file will be instructions and guidance on how to activate, navigate and use the AI chatbot.
These sections will be divided into their corresponding code blocks which'll be indicated at the beginning of each section in the format: "# 1"
Please run these sections chronologically for initial set up.

Section 1:
- Downloads all the appropriate packages
- Ensure ngrok is correctly authenticated and configured

Section 2:
- Imports all appropriate packages
- Output should display: Mounted at /content/drive

Section 3:
- The download and initialization of required models

Section 4:
- The retrieval of data from data.csv and storage in question_embeddings

Section 5:
- Initialization of is_medical() function

Section 6:
- Initialization of generate_response() function

Section 7:
- Initialization of application and HTML template

Section 8:
- Creation of feedback.db database on Google Drive if it doesn't already exist

Section 9:
- Displays last 10 previous feedback entries
- Doesn't need to be ran for initial set up. Can be run whenever web application is closed 

Section 10:
- Starts and begins running the application
- In order to access the chatbot UI. Follow the link provided at "Public URL: ..."
- You'll be taken to a secondary webpage where you then press "Visit page"


KEY NOTES:
- In order to exit the program, please first close the UI and then stop running Section 10.
- In order to run the application again, please first run Section 7 and then Section 10.
Note. Section 10 will display an error if Section 7 has not been ran prior.