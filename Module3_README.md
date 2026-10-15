# Module 3: LLM APIs & Application Development

## Project: AI Chat Application using Gemini API

A beginner-friendly AI chat application built in Python with Google Colab, the Gemini API, and Gradio. The app accepts user messages, returns AI responses, displays chat history during the active session, and lets users provide custom instructions.

## Features

- Connects to the Gemini API using the Google Gen AI Python SDK.
- Reads the API key from Google Colab Secrets (`GEMINI_API_KEY`) rather than hard-coding it in the notebook.
- Provides a Gradio chat interface.
- Keeps recent messages as context during the active session.
- Supports custom instructions for response style.
- Includes a Clear Chat button.
- Demonstrates structured JSON output validated with Pydantic.
- Displays input, output, and total token usage when returned by the API.
- Handles common API errors with readable messages.

## Tools and Technologies

- Python
- Google Colab
- Gemini API
- `google-genai`
- Gradio
- Pydantic

## How to Run

1. Open `Module3_AI_Chat_Application.ipynb` in Google Colab.
2. Add your Gemini API key in Colab Secrets with the exact name `GEMINI_API_KEY`.
3. Enable notebook access for that secret.
4. Run the notebook cells in order, installing required packages where instructed.
5. Start the Gradio app and open the temporary link printed in the output.
6. Keep the Colab runtime running while using the temporary app link.

## Testing Checklist

- [ ] Send a message and receive a Gemini response.
- [ ] Ask a follow-up question and confirm recent chat history is used.
- [ ] Change custom instructions and check the response style.
- [ ] Clear the conversation.
- [ ] Generate and validate a structured JSON response.
- [ ] Display input, output, and total token counts.
- [ ] Test error handling and record the actual result.

Mark checklist items only after testing them in your notebook.

## Security and Cost Notes

- Never commit or publish your API key. Keep it in Colab Secrets.
- A Gradio share link is temporary and may be accessible to anyone who has the link while the app is running. Do not enter sensitive information.
- API usage may be subject to quota limits or charges depending on account, model, and current pricing. Check Google AI Studio for current limits and pricing.
- Limit response length and the amount of conversation history sent to manage token usage.

## Important Note

This project is intended for learning and demonstration. Temporary Colab and Gradio sessions stop when the runtime ends, so the share link is not a permanent deployment URL.
