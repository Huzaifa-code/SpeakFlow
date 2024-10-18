# SpeakFlow

Welcome to **SpeakFlow** – Effortlessly convert your speech into text and translate it into any language, all from the web!

![SpeakFlow](https://i.imgur.com/apsQ1yI.png)

## Overview

SpeakFlow is a React-based web application that leverages web workers to run machine learning models directly in your browser. It uses `transformers.js` to perform speech-to-text transcription and supports translation into multiple languages.

### Key Features:
- **Real-Time Speech-to-Text**: Convert your audio input into text quickly and efficiently.
- **Translation**: Translate the transcribed text into any supported language.
- **Browser-Based ML**: No server required! The app runs ML models in the browser using web workers.
- **Asynchronous Processing**: Perform tasks like downloading, loading, and inference in the background, ensuring smooth user experience.

## How It Works
- The app uses **web workers** to handle background tasks, ensuring the UI remains responsive while models are downloaded, loaded, and processed.
- You can upload an audio file or provide live audio input. The audio is decoded and sent to the worker, which runs the **Whisper model** from Hugging Face using `transformers.js`.
- Once the transcription is complete, you can see the results and optionally translate the text.

## Tech Stack
- **React**: For building the user interface.
- **Vite**: As the build tool for fast development.
- **Tailwind CSS**: For styling and layout.
- **Transformers.js**: A browser-compatible version of Hugging Face's transformers for running ML models.
- **Web Workers**: For running tasks in the background without blocking the UI.

## Installation and Usage

To get started locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-repo/speak-flow.git
   cd speak-flow
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Run the app**:
   ```bash
   npm run dev
   ```

4. **Build for production**:
   ```bash
   npm run build
   ```

## Screenshot
![Screenshot](https://i.imgur.com/apsQ1yI.png)

## Dependencies
- `@xenova/transformers`: For running Hugging Face models in the browser.
- `react`: For building the user interface.
- `vite`: For fast builds and development.
- `tailwindcss`: For styling and responsive layouts.
- `web workers`: For running the Whisper model asynchronously.

### Supported Tasks:
- **Speech Recognition**: Convert audio to text using Whisper.
- **Translation**: Translate text to any language using `transformers.js`.
- **Natural Language Processing (NLP)**: Leverage state-of-the-art models for tasks like summarization, text generation, and more.

## Resources
- [@xenova/transformers on npm](https://www.npmjs.com/package/@xenova/transformers)
- [Hugging Face Models](https://huggingface.co/models)

