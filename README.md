# Building a Real-Time AI Voice Assistant on an ESP32 with OpenAI and Langchain
Hey everyone!

I've been working on a super exciting project over the past couple of weeks and couldn't wait to share it with this community.

I've built a real-time voice assistant using an ESP32 microcontroller, use as an I/O interface, integrated with a Node Server that uses **LangChain** and **OpenAI**.

**Overall Architecture:**

* A voice assistant that you can interact with in real-time.
* Uses an ESP32 for audio input/output.
* Integrates with a Node.js server powered by LangChain and OpenAI.
* Supports real-time audio streaming via WebSockets.
* You can use it with any Langchain Tools or Agent

**Why I Built It:**

* To explore the possibilities of interaction with an agent from a connected device
* To have a hands-on project that combines hardware and software development.
* Because I thought it would be cool to talk to my own AI assistant anytime by just pressing a button! Actually it is, the interaction is quite fluent, and it doesn't monopolize your computer or smartphone, like an app.

* And for course, have a look at the [code repository](https://github.com/Mostafizur-99/Voice-Assistance).

# Project Highlights 

* **Hardware Components:**
   * **ESP32-S3 Development Board:** The brain of the assistant.
   * **I²S Digital Microphone (INMP441):** Capturing voice input.
   * **I²S Amplifier (MAX98357A):** Driving the speaker output.
   * **Small Speaker (3W, 4Ω):** For audio responses.
   * **Push Button & Resistors:** To initiate recordings.
   * **Jumper Wires & Breadboard:** For connections.

* **Software Implementation:**
   * **ESP32 Firmware (C++):** Handles audio capture, buffer management, and WebSocket communication.
   * **Node.js Server (TypeScript):** Manages AI processing using LangChain and OpenAI's APIs.
   * **Real-Time Audio Streaming:** Efficient buffer handling to ensure smooth data flow.

# How It Works 

1. **Voice Capture:** Press the button on the ESP32 to start recording your voice.
2. **Data Transmission:** Audio data is sent via WebSockets to the Node.js server.
3. **AI Processing:** The server uses LangChain and OpenAI to transcribe and understand your speech, then generates a response.
4. **Response Playback:** The audio response is sent back to the ESP32 and played through the speaker.



**GitHub Repository:** [ESP32 Reatime Voice AI Assistant](https://github.com/Mostafizur-99/Voice-Assistance)

You should be able to replicate the project and customize it for your needs.

# Future Improvements 

* **Enhance Audio Processing:** Implement automatic start/stop of discussion, withouth pressing a button, interrupt the assistant, improve output (as far as it's possible to maintain a 44100kbps
* **Expand AI Capabilities:** Add more tools and commands for the assistant.
* **Optimize Performance:** Fine-tune buffer sizes and network handling.

# Feedback and Collaboration 🤝

I'm really looking forward to hearing your thoughts on this project. Whether it's suggestions for improvements, ideas for new features, or any questions you might have—let's discuss!

If anyone's interested in collaborating or contributing, feel free to fork the repository or reach out.

**TL;DR:** I built a DIY real-time voice assistant using an ESP32, integrated with LangChain and OpenAI. It captures voice input, sends it to a Node.js server for AI processing, and plays back the response—all in real-time! Check out the [video ](https://www.youtube.com/watch?v=1H6FlWNRSYM)or the project on [GitHub ](https://github.com/FabrikappAgency/esp32-realtime-voice-assistant)and let me know what you think!

**Cross-posting to:** r/esp32, r/LangChain, r/arduino 

*Excited to hear your feedback!* 😊
