# AI Image Description & Translation Web App

This project is a Streamlit-based web application that allows users to:

✅ Upload an image

✅ Provide a custom prompt

✅ Generate AI-based descriptions using Google Gemini

✅ Convert the generated text into speech (TTS)

✅ Translate the description into multiple Indian languages

🚀 Features
1. Image Upload

Users can upload .jpg images for processing.

2. Prompt-Based Description

A custom prompt is sent along with the uploaded image to generate a detailed description using:

Google Generative AI (Gemini 1.5 Flash)

3. Voice Generation (Text-to-Speech)

The app uses pyttsx3 to convert the generated description into:

Male Voice

Female Voice

And saves the audio as 1.mp3.

4. Multi-Language Translation

Using googletrans, the generated text can be translated to:

English

Hindi

Odia

Telugu

Tamil

Punjabi

Malayalam

Marathi

5. Memory Optimization

Streamlit’s session_state ensures the description is not re-generated unnecessarily.

🛠️ Technologies Used
Module / Library	Purpose
Streamlit	Web app interface
Google Generative AI (Gemini)	Image description generation
Pillow (PIL)	Image processing
pyttsx3	Text-to-speech
googletrans	Language translation
asyncio	Async handling
📦 Installation
1. Clone the repository
git clone https://github.com/your-username/ai-image-description.git
cd ai-image-description

2. Create a virtual environment (optional but recommended)
python -m venv venv
source venv/Scripts/activate   # Windows

3. Install dependencies
pip install -r requirements.txt

4. Add your Gemini API Key

Replace inside the code:

api_key = "YOUR_API_KEY"


Or use a .env file.

▶️ Running the Application

Run the Streamlit server:

streamlit run app.py


This will open the app in your default browser at:

http://localhost:8501

📁 Project Structure
├── app.py
├── README.md
├── requirements.txt
└── 1.mp3 (generated at runtime)

📝 How It Works

User uploads an image and enters a prompt

The app sends both to the Gemini API

The model returns a description

User can:

Listen to the description (TTS)

Translate it into various languages

Everything runs inside Streamlit interface

⚠️ Important Notes

Google Gemini API key is required for the app to work

pyttsx3 may behave differently based on system voice installation

Translation quality depends on googletrans library

📜 License

This project is open-source. Use it freely for learning or extension.
