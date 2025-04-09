Mood-Based Music Recommendation Bot

**Sofi** is a conversational music recommendation system that analyzes a user's mood from natural language conversations and suggests songs accordingly. It uses emotion detection, NLP, and a friendly chatbot interface to match the right music to your vibe.

---

## Overview

This project uses a Large Language Model (LLM) to:
- Engage in conversation with users
- Detect mood/emotions from text using sentiment analysis
- Recommend music tracks or playlists that align with the user's feelings

It’s a unique blend of AI-powered conversation and music discovery – perfect for integrating into websites, apps, or mental wellness tools.

---

## Features

- **Mood Analysis**: Detects user emotions through open-ended chat.
- **Song Recommendations**: Suggests music with links and short explanations.
- **Emoji/Slang Support**: Recognizes feelings expressed in casual language.
- **Conversation Memory**: Context-aware suggestions powered by Cohere’s `chat` model.
- **Fallback Suggestions**: Offers chill playlists even if mood is unclear.
- **Streamlit UI**: Interactive and simple web interface.

---

## Technologies Used

- Python
- [Cohere](https://cohere.com/) API (LLM)
- Streamlit (Web UI)
- Prompt Engineering for emotional context
- Optional: Web Search Connector (via Cohere)

---

## Installation

### Prerequisites

- Python 3.7+
- Cohere API key (Get it [here](https://dashboard.cohere.com/))

### Setup

1. Clone the repository:
```bash
git clone https://github.com/heisenberg2358/music-mood-bot.git
cd music-mood-bot
Install dependencies:
pip install -r requirements.txt

Add your Cohere API key in app.py:
co = cohere.Client('YOUR_API_KEY')

Run the app with Streamlit:
streamlit run app.py
Then open http://localhost:8501 in your browser.

Example Conversation

User: I’ve been feeling a little low lately.
Sofi: That sounds tough. Here's a feel-good track to lift you up:  
“Happy – Pharrell Williams”  
[https://youtu.be/ZbZSe6N_BXs]

How It Works
A custom prompt guides the LLM to behave like a Music Mood Buddy

User input is evaluated for emotional signals (e.g., “tired”, “vibing”, “heartbroken”)

A recommendation engine maps moods to curated songs/playlists

Conversations are maintained with st.session_state for coherence

To-Do / Future Plans
Integrate Spotify API for dynamic playlist generation

Add voice input and speech-to-text mood analysis

Create a feedback system for learning user preferences

Save favorite songs per user session

Contribution
Have a new idea or want to improve song matching? Feel free to fork and contribute.

License
This project is licensed under the MIT License.

Contact
For any queries or suggestions:
Email: [ajumalsabeer350@gmail.com]
GitHub: [https://github.com/heisenberg2358/music-mood-bot]





