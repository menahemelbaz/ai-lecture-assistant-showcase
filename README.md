<p align="center">
  <img src="assets/logo.png" alt="AI Lecture Assistant Logo" width="180">
</p>

# AI Lecture Assistant

AI Lecture Assistant is a Chrome extension designed to help students study recorded lectures more efficiently.

It provides tools for generating lecture summaries, chatting with an AI assistant based on the lecture transcript, and practicing lecture topics.

The extension works while the user watches a recorded lecture and uses the lecture content to provide learning tools that make reviewing and understanding the material easier.

> This repository is a project showcase only. The source code is kept private.

## Features

* Lecture summary PDF generation
* AI chat based on the lecture transcript
* Lecture topic practice

## Tech Stack

* TypeScript
* JavaScript
* Node.js
* Express.js
* Web Audio API
* OpenAI API
* WebSocket
* Chrome `tabCapture`
* Offscreen Documents

## Screenshots

### Main Extension Button

The extension adds a floating button on top of the lecture page, allowing the user to access the study tools while watching the lecture.

<img src="assets/main-button.png" alt="Main Extension Button" width="350">

### Study Tools Menu

The extension provides quick access to the main learning tools: lecture summaries, lecture-based AI chat, and practice questions.

<img src="assets/feature-buttons.png" alt="Study Tools Menu" width="300">

### Summary Generation

The extension allows the user to generate a lecture summary while watching the recorded lecture.

<img src="assets/summary-process.png" alt="Summary Generation" width="700">

### Lecture-Based AI Chat

The chat interface allows students to ask questions about the lecture while watching, based on the accumulated lecture transcript.

<img src="assets/chat-panel.png" alt="Lecture-Based AI Chat" width="700">

## Architecture

The project is divided into two main parts:

* **Chrome Extension** - Provides the user interface, manages the lecture flow, captures lecture audio, and communicates with the backend.
* **Node.js Server** - Handles transcription, AI-based summary generation, lecture Q&A, practice generation, PDF creation, and real-time communication.

The full implementation is organized into modular components for content scripts, background logic, offscreen audio processing, server routes, and backend services.

## Status

This project is a working prototype and personal learning project focused on Chrome Extensions, backend development, audio processing, and AI integration.

The public repository is intended to present the project concept, features, and screenshots. The source code is not included.
