# Multilingual Voice AI Tutor using Whisper and LLMs

An AI-powered voice tutor that enables users to communicate naturally through speech. The system converts spoken input into text, generates intelligent responses using an LLM, and converts the response back into speech in the detected language.

The project combines **Speech AI, Large Language Models, and Text-to-Speech** to create an interactive multilingual learning assistant.

---

## Features

### Speech-to-Text Conversion

* Converts user voice input into text
* Uses Faster-Whisper for accurate speech recognition
* Automatically detects the spoken language

### AI Conversation Engine

* Uses Groq API with Llama 3.3 for response generation
* Maintains a tutor-style conversational behavior
* Provides:

  * Grammar corrections
  * Short explanations
  * Natural conversation practice
  * Follow-up questions

### Text-to-Speech Response

* Converts AI-generated responses into voice
* Generates speech in the detected language
* Enables real-time voice interaction

### Multilingual Support

* Automatically detects input language
* Replies in the same language
* Supports language learning conversations

---

## System Architecture

```
User Voice Input
        |
        ↓
Speech Recognition
(Faster-Whisper)
        |
        ↓
Language Detection
        |
        ↓
LLM Processing
(Groq API + Llama 3.3)
        |
        ↓
AI Generated Response
        |
        ↓
Text-to-Speech
(gTTS)
        |
        ↓
Voice Output
```

---

## Tech Stack

### Programming

* Python

### AI / ML

* Large Language Models (LLMs)
* Speech Recognition
* Natural Language Processing
* Multilingual AI

### Libraries

* Faster-Whisper
* Groq SDK
* gTTS
* Langdetect

### APIs

* Groq API

---

## Workflow

1. User provides voice input
2. Audio is processed using Whisper speech recognition
3. Speech is converted into text
4. Language is automatically detected
5. Text is sent to LLM for generating a response
6. AI response is converted into speech
7. User receives voice output

---

## Installation

Clone repository:

```bash
git clone YOUR_REPOSITORY_LINK

cd Multilingual-Voice-AI-Tutor
```

Install dependencies:

```bash
pip install -r requirements.txt
```

---

## Environment Setup

Create a `.env` file:

```env
GROQ_API_KEY=your_api_key_here
```

Load the key in Python:

```python
from dotenv import load_dotenv
import os

load_dotenv()

api_key = os.getenv("GROQ_API_KEY")
```

---

## Run Project

```bash
python main.py
```

---

## Project Pipeline

```
Audio
 ↓
Whisper Model
 ↓
Text
 ↓
LLM Response Generation
 ↓
gTTS
 ↓
Audio Output
```

---

## Future Improvements

* Add user progress tracking
* Add conversation memory
* Improve voice quality with advanced TTS models
* Add web interface using Streamlit
* Add pronunciation scoring
* Add real-time streaming conversation

---

## Author

Poorva Jain

GitHub:
https://github.com/poorvajain04
