# ESP32 Voice-Controlled Timer

A countdown timer on a Seeed XIAO ESP32-S3 Sense, built in two stages: first controlled by covering a light sensor, then by spoken commands recognized on the board itself.

![Timer states: STANDBY, ADDING, COUNTDOWN](a2-voice-commands/media/voice-timer-states.jpg)

▶️ **[Watch the voice demo (58 s, with sound)](a2-voice-commands/media/voice-timer-demo.mp4)**

| Part | What it adds |
|---|---|
| [**A1: Light-controlled gesture timer**](a1-light-timer/) | Self-calibrating light sensing, tap/hold gesture detection, and a non-blocking four-state timer |
| [**A2: Voice commands**](a2-voice-commands/) | On-device keyword spotting feeding a C++ armed/latched command policy (0.90 accept threshold at 97% precision), driving the same timer |

**Hardware:** Seeed XIAO ESP32-S3 Sense (onboard microphone), GL5528 photoresistor, LEDs, breadboard
**Tools:** C++ (Arduino framework), Arduino IDE, Python / Google Colab

Built for ECE 116 at UC San Diego.
