# Language Translator

This project is a versatile language translation tool that can translate spoken or written
phrases. It's set up for Brazilian Portuguese by default, but you can change this to any
language by modifying the worker.py file.

## Project Overview

This application acts as a communication bridge. It converts spoken audio into text
and then translates that text, or directly translates written input. It uses IBM Watson
services for Speech-to-Text and Text-to-Speech to provide a complete translation
experience.

## Setup and Installation

To get this project up and running, you will install dependencies locally.

**Prerequisites**

```
● Python 3.8+
● pip (Python package installer)
```
**Configuration**

You **must** set up your API keys and service URLs before running the application. These
sensitive details are loaded from environment variables for security.

1. **Create a** ```.env``` **file** : In your project's root directory, create a file named .env.
2. **Add your credentials** : Fill the .env file with your IBM Watson API keys and service
    URLs. Replace the placeholder values with your actual credentials:
```
    WATSON_SPEECH_TO_TEXT_API_KEY=YOUR_SPEECH_TO_TEXT_API_KEY_HERE
    WATSON_SPEECH_TO_TEXT_URL=YOUR_SPEECH_TO_TEXT_URL_HERE
    WATSON_TEXT_TO_SPEECH_API_KEY=YOUR_TEXT_TO_SPEECH_API_KEY_HERE
    WATSON_TEXT_TO_SPEECH_URL=YOUR_TEXT_TO_SPEECH_URL_HERE
    MODEL_API_KEY=YOUR_MODEL_API_KEY_HERE
    MODEL_PROJECT_ID=YOUR_MODEL_PROJECT_ID_HERE
```
You can get these API keys and URLs by creating the services on IBM Cloud:
○ IBM Watson Speech-to-Text : https://www.ibm.com/products/speech-to-text
○ IBM Watson Text-to-Speech : https://www.ibm.com/products/text-to-speech
For help getting the Project ID and API Key for your model, see this article:
○ IBM Watsonx AI - The Interface and API :
https://medium.com/the-power-of-ai/ibm-watsonx-ai-the-interface-and-api-
e8e1c

**Installation**

1. **Clone the repository** :
```
    git clone https://github.com/vitor115/translator_AI_Assistant.git
    cd translator_AI_Assistant
```
2. **Install dependencies** :
```
    pip install -r requirements.txt
```

## Usage

Once the application is running, follow its output or UI (if applicable) to interact with
the translator.

## Customization

The default language for translation (Brazilian Portuguese) can be changed. Look for
relevant configuration or prompt settings in the worker.py file to adjust source or target
languages.


