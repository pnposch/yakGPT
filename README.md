# YakGPT

A simple, locally running ChatGPT UI that makes your text generation faster and chatting even more engaging!

[![yakgpt.com](https://img.shields.io/badge/visit-website-green.svg?style=for-the-badge)](https://yakgpt.vercel.app)

## Features

-   Run locally on browser – no need to install any applications
-   Faster than the official UI – connect directly to the API
-   Easy mic integration – no more typing!
-   Use your own API key – ensure your data privacy and security

-   All state stored locally in localStorage – no analytics or external service calls
-   Access on https://yakgpt.vercel.app or run locally!

## 🚀 Getting Started

Visit [YakGPT](https://yakgpt.vercel.app) to try it out without installing, or follow these steps to run it locally:

### Prerequisites

You'll need the following tools installed on your computer to run YakGPT locally.

-   [Git](https://git-scm.com/)
-   [Yarn](https://yarnpkg.com/) (or npm or pnpm)
-   Any modern web browser like Google Chrome, Mozilla Firefox, or Microsoft Edge

### Installation

1. Clone the repository:

```
$ git clone https://github.com/your-username/YakGPT.git
```

2. Install dependencies, build the bundle and run the server

```
$ yarn
$ yarn build
$ yarn start
```

Congratulations! 🎉 You are now running YakGPT locally on your machine.

## 🔑 API Key Configuration

To utilize YakGPT, you'll need to acquire an API key for OpenAI. The app should prompt you to insert you key.

## 🐳 Docker

To build a Docker image, run:

```
docker build -t yakgpt:latest .
```

To run in a container:

```
docker run -p 3000:3000 yakgpt:latest
```

## 🎤 Microphone Integration

YakGPT makes chatting a breeze with its microphone integration! Activate your microphone using your browser's permissions, and YakGPT will automatically convert your speech into text.

You can also toggle the mic integration as needed by clicking on the microphone icon in the app.

Remember to use a supported web browser and ensure your microphone is functioning properly.

## 🛡️ Data Privacy and Security

YakGPT ensures your data privacy and security by letting you use your own API key. Your conversation with YakGPT takes place directly between your browser and OpenAI's GPT-3 API, with no intermediary servers.

## 📃 License

This project is licensed under the MIT License - see the [`LICENSE`](LICENSE) file for details

## 🙌 Acknowledgments

-   [OpenAI](https://openai.com/) for building such amazing models and making them cheap as chips.
-   [opus-media-recorder](https://github.com/kbumsik/opus-media-recorder) A real requirement for me was to be able to walk-and-talk. OpenAI's Whisper API is unable to accept the audio generated by Safari, and so I went back to wav recording which due to lack of compression makes things incredibly slow on mobile networks. `opus-media-recorder` saved my butt by allowing cross-platform compressed audio recording via web worker magic. 🤗

Got feedback, questions or ideas? Feel free to submit an issue!
