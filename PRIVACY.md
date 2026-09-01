# Privacy Policy for AI Lecture Assistant

Last updated: September 1, 2026

AI Lecture Assistant is a Chrome extension that captures audio from a user-selected browser tab, transcribes lecture content, and uses the transcript to generate summaries, answers, and practice questions.

## Information Handled by the Extension

AI Lecture Assistant handles the following information:

* The user's personal OpenAI API key.
* Audio captured from the browser tab selected by the user.
* Transcripts generated from the captured audio.
* Questions submitted through the lecture chat and the generated answers.
* Lecture-related information, including the page URL, page title, video source URL, and video duration.
* Temporary extension state needed to manage the active recording session.

The extension does not capture microphone audio.

## How the Information Is Used

The information is used only to provide the extension's study features:

* Tab audio is sent to OpenAI for transcription.
* Transcripts are sent to OpenAI to generate summaries, answers, topics, and practice questions.
* The OpenAI API key is used only to authenticate requests made directly to OpenAI.
* Lecture information is used locally to identify and manage the active lecture session.

The developer does not operate an intermediate server and does not receive the user's API key, audio, transcript, questions, or generated content.

## Local Storage

The OpenAI API key is stored locally using Chrome extension storage and remains stored until the user removes it from the extension settings or uninstalls the extension.

The active transcript, lecture information, chat history, and recording state are also stored locally. They are cleared when the user ends the active session or starts a new lecture session.

Raw audio is buffered temporarily in memory for transcription and is not stored permanently by the extension.

## Third-Party Services

AI Lecture Assistant sends information directly to OpenAI:

* The user's API key is included in authenticated API requests.
* Captured tab audio is sent for transcription.
* Transcripts and user questions are sent to generate study content.

OpenAI processes this information according to its own terms and privacy policies.

When the extension interface is activated, visual resources may also be requested from Google Fonts and cdnjs. These providers may receive standard technical request information such as the user's IP address, browser information, and referring website origin. They do not receive the user's API key, captured audio, transcript, or chat content from the extension.

## Data Selling, Advertising, and Analytics

AI Lecture Assistant does not:

* Sell user data.
* Use user data for advertising.
* Use analytics or tracking services.
* Transfer user data to data brokers.
* Allow the developer or other humans to read the user's lecture content.

## Security

All requests containing user data are transmitted over HTTPS. The extension limits the use of information to the features described in this policy.

Users are responsible for keeping their OpenAI API key secure and should remove or revoke it if they believe it has been exposed.

## User Choices and Data Deletion

Users can:

* Remove their stored OpenAI API key from the extension settings.
* End the active lecture session to clear its transcript and chat history.
* Uninstall the extension to remove locally stored extension data.
* Revoke their API key through the OpenAI Platform.

## Limited Use

AI Lecture Assistant's use of information received through Chrome APIs adheres to the Chrome Web Store User Data Policy, including the Limited Use requirements. User information is used only to provide the extension's disclosed, user-facing features.

## Changes to This Policy

This policy may be updated if the extension's features or data practices change. The “Last updated” date at the top of this page will reflect the latest revision.

## Contact

For questions about this privacy policy or the extension's data practices, contact:

elbazmm7700@gmail.com
