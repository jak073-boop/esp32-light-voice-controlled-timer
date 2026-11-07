# ESP32 Voice-Controlled Timer

A countdown timer on a Seeed XIAO ESP32-S3 Sense, built in two stages: first controlled by covering a light sensor, then by spoken commands recognized on the board itself.

![Timer states: STANDBY, ADDING, COUNTDOWN](a2-voice-commands/media/voice-timer-states.jpg)



https://github.com/user-attachments/assets/a7bdf088-a06f-4376-9ed7-a8e3b965b493



| Part | What it adds |
|---|---|
| [**Light-controlled gesture timer**](a1-light-timer/) | Self-calibrating light sensing, tap/hold gesture detection, and a non-blocking four-state timer |
| [**Voice commands**](a2-voice-commands/) | On-device keyword spotting feeding a C++ armed/latched command policy (0.90 accept threshold at 97% precision), driving the same timer |

**Hardware:** Seeed XIAO ESP32-S3 Sense (onboard microphone), GL5528 photoresistor, LEDs, breadboard
**Tools:** C++ (Arduino framework), Arduino IDE, Python / Google Colab

Built for ECE 116 at UC San Diego.
