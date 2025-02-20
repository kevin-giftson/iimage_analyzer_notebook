# Medical Image Analysis using Google Gemini API

## Overview
This project utilizes Google's Gemini AI (Generative AI) to analyze medical images. The AI model assists in detecting anomalies, diseases, or other health-related issues in medical images, providing structured insights.

## Features
- **Automated Image Analysis**: Uses Google's Gemini AI to process and analyze medical images.
- **Structured Report Generation**: Provides findings in a structured format.
- **Next Steps and Treatment Suggestions**: Offers recommendations based on detected issues.
- **Doctor Consultation Reminder**: Ensures professional medical advice is prioritized.

## Setup Instructions
### 1. Clone the Repository
```bash
git clone https://github.com/your-repo-name.git
cd your-repo-name
```

### 2. Create a Virtual Environment (Optional but Recommended)
```bash
python -m venv venv
source venv/bin/activate  # On Windows use: venv\Scripts\activate
```

### 3. Install Dependencies
```bash
pip install -r requirements.txt
```

### 4. Configure the API Key
- Obtain an API Key from **[Google AI Studio](https://makersuite.google.com/)**.
- Enable the **Google Generative AI API** in **Google Cloud Console**.
- Set up your API key in the environment:
```python
import google.generativeai as genai
API_KEY = "your_api_key_here"
genai.configure(api_key=API_KEY)
```

Alternatively, set it as an environment variable:
```bash
export GOOGLE_API_KEY="your_api_key_here"  # For Linux/macOS
set GOOGLE_API_KEY="your_api_key_here"  # For Windows
```

### 5. Run the Script
```bash
python main.py  # Ensure the script is pointing to the correct file name
```

## Common Issues & Troubleshooting
### Invalid API Key Error
- Ensure your API key is correctly set.
- Verify that the **Generative AI API** is enabled in your Google Cloud Console.
- Try regenerating a new API key in **Google AI Studio**.

### Image Processing Issues
- Ensure the image is clear and relevant to human health.
- If the image quality is poor, the AI may return **'Unable to determine based on provided images'**.

## Disclaimer
The AI-generated analysis is not a substitute for professional medical advice. **Consult with a doctor before making any decisions.**

