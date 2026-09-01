<p align="center">
  <img src="assets/logo.png" alt="AI Lecture Assistant Logo" width="180">
</p>

# AI Lecture Assistant

AI Lecture Assistant is a Chrome extension designed to help students study recorded lectures more efficiently.

It captures lecture audio while the user watches a recorded video, builds a transcript, and uses the lecture content to support review and practice.

The extension provides tools for generating printable lecture summaries, asking questions based on the active transcript, and practicing lecture topics with immediate feedback.

All AI features run directly against the user's personal OpenAI API key from within the extension — the project no longer requires a backend server.

## Features

* Printable lecture summary generation
* AI chat based on the active lecture transcript
* Topic-based practice questions with feedback and explanations

## Configuration

The extension settings page allows users to add, update, or remove their personal OpenAI API key. The key is stored locally in Chrome extension storage and is used only for direct requests to OpenAI. On first install, the settings page opens automatically so the user can add their key before using the extension.

<img src="assets/api-key-settings.png" alt="OpenAI API Key Settings" width="800">

## Screenshots

### Main Extension Button

The extension adds a floating button to the lecture page, allowing the user to access the study tools while watching the lecture.

<img src="assets/main-button.png" alt="Main Extension Button" width="350">

### Study Tools Menu

The extension provides quick access to lecture summaries, lecture-based AI chat, and practice questions.

<img src="assets/feature-buttons.png" alt="Study Tools Menu" width="300">

### Summary Generation

The extension generates a formatted lecture summary that can be printed or saved as a PDF.

<img src="assets/summary-process.png" alt="Summary Generation" width="700">

### Lecture-Based AI Chat

The chat interface allows students to ask questions based on the accumulated transcript of the active lecture.

<img src="assets/chat-panel.png" alt="Lecture-Based AI Chat" width="700">

### Practice Questions

The practice interface generates questions from lecture topics and provides immediate feedback with explanations.

<img src="assets/practice-questions.png" alt="Lecture Practice Questions" width="700">

## Tech Stack

* TypeScript
* Chrome `tabCapture`
* Offscreen Documents
* Web Audio API
* OpenAI API (Whisper transcription and chat models)

## Architecture

The extension runs entirely on the client. It provides the user interface, coordinates tab-audio capture, manages lecture sessions, transcribes audio, and generates transcript-based study tools.

Captured audio is transcribed by calling the OpenAI transcription API directly from the offscreen document. Summaries, chat answers, and practice questions are produced by calling the OpenAI chat API directly from the background service worker. All requests use the user's personal API key, and no lecture data passes through any intermediate server.

The codebase is organized into modular components for content scripts, background logic, offscreen audio processing, transcript storage, and AI-powered learning features.
