# Ujjwala Voice Help

Ujjwala Voice Help is a free, voice-first prototype designed to help users interact with information about the Pradhan Mantri Ujjwala Yojana using speech.

## Features

- Voice-based interaction using the browser's Speech Recognition API.
- Text-to-speech responses using the browser's Speech Synthesis API.
- Supports six Indian language options:
  - English
  - தமிழ் (Tamil)
  - हिन्दी (Hindi)
  - తెలుగు (Telugu)
  - ಕನ್ನಡ (Kannada)
  - മലയാളം (Malayalam)
- Displays what the user said.
- Displays the assistant's response.
- Provides visual states for listening and speaking.
- Does not require an API key.
- Includes an error message when speech recognition is unavailable or the speech cannot be understood.

## How It Works

1. Select a language from the language menu.
2. Tap the microphone button.
3. Speak your question or statement.
4. The browser converts the speech into text.
5. The application displays the recognized speech.
6. The prototype selects a predefined response based on the selected language and recognized keywords.
7. The response is displayed and spoken aloud in the selected language.

## Supported Languages

| Language | Speech Recognition Code |
|---|---|
| English | `en-IN` |
| Tamil | `ta-IN` |
| Hindi | `hi-IN` |
| Telugu | `te-IN` |
| Kannada | `kn-IN` |
| Malayalam | `ml-IN` |

## Technologies Used

- HTML5
- CSS3
- JavaScript
- Web Speech API
  - Speech Recognition
  - Speech Synthesis

## Project Structure

```text
Ujjwala-Voice-Help/
└── index.html
```

The current prototype is contained in a single `index.html` file.

## How to Run

### Option 1: Open Locally

1. Download or copy the project files.
2. Open `index.html` in a supported web browser.
3. Select your preferred language.
4. Tap the microphone.
5. Allow microphone access if the browser asks for permission.
6. Speak and wait for the response.

### Option 2: Deploy Online

The project can be deployed using a static web-hosting service. Upload the `index.html` file to the hosting service and open the generated project URL in a supported browser.

## Browser Compatibility

The application uses browser speech-recognition functionality. The code checks for:

```javascript
window.SpeechRecognition || window.webkitSpeechRecognition
```

If speech recognition is unavailable, the application displays an error asking the user to use Chrome on Android or Chrome on a computer.

## Current Prototype Logic

The current version uses predefined responses for each supported language. It checks the recognized speech for selected gas/connection-related keywords and chooses one of two predefined responses.

This means the current prototype is **not a general AI chatbot** and does not connect to a live government database or external Ujjwala API.

## Limitations

- Speech recognition depends on browser support.
- Recognition accuracy can vary depending on the device, microphone, environment, accent, and background noise.
- The current responses are predefined.
- The prototype does not verify a user's eligibility or application status.
- The application does not connect to an official Ujjwala database.
- Users should verify official scheme rules before relying on information provided by the prototype.

## Future Improvements

Possible improvements include:

- Add more Ujjwala-related questions and answers.
- Add more Indian languages.
- Improve natural-language understanding.
- Connect the application to verified official scheme information.
- Add an accessibility-friendly interface.
- Add offline or low-connectivity support where technically possible.
- Improve speech recognition for noisy environments.
- Add a guided application process.
- Add links to official government resources.

## Disclaimer

This is a prototype for the Pradhan Mantri Ujjwala Yojana. It should not be treated as an official government application or source. Always verify current scheme rules and eligibility requirements through official sources before making decisions.

## License

No specific open-source license is currently specified for this prototype.
