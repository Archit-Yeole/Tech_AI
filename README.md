# Tech_ai_chatbot


This is a simple chatbot built using Flask and Google Gemini API. It allows users to input text and receive AI-generated responses using Google's Gemini model.

## Features
- Accepts user input via a web interface.
- Sends requests to the Google Gemini API to generate responses.
- Returns AI-generated responses in JSON format.
- Handles errors gracefully, including missing API keys and invalid responses.

## Prerequisites
- Python 3.7+
- Flask
- Requests library
- A valid Google Gemini API key

## Installation
1. Clone this repository:
   ```sh
   git clone https://github.com/yourusername/flask-gemini-chatbot.git
   cd flask-gemini-chatbot
   ```
2. Create a virtual environment (optional but recommended):
   ```sh
   python -m venv venv
   source venv/bin/activate  # On Windows use: venv\Scripts\activate
   ```
3. Install dependencies:
   ```sh
   pip install flask requests
   ```
4. Set up your Google Gemini API key as an environment variable:
   ```sh
   export GEMINI_API_KEY="your_api_key_here"  # On Windows use: set GEMINI_API_KEY="your_api_key_here"
   ```

## Usage
1. Start the Flask server:
   ```sh
   python app.py
   ```
2. Open your browser and go to:
   ```
   http://localhost:10000/
   ```
3. Enter text and receive responses from the AI.

## API Endpoint
- **POST** `/generate`
  - **Request:** JSON with `inputText`
  - **Response:** JSON with AI-generated response or error message
  
Example Request:
```json
{
    "inputText": "Hello, how are you?"
}
```
Example Response:
```json
{
    "response": "I'm doing great! How can I assist you today?"
}
```

## Deployment
To deploy this Flask app, use services like:
- **Render**


Make sure to configure the `GEMINI_API_KEY` as an environment variable in your deployment platform. or add it manually


# Tech_AI
