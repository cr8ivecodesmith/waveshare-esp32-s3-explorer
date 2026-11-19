# Project ideas

Pick whatever sounds interesting. These are invitations, **not assignments**, and they are not implemented examples in this repository.

A small success can be as simple as changing a label on screen or playing a sound in response to a button press.

## First modifications

| Idea | Uses | Possible starting point |
| --- | --- | --- |
| Personal badge or greeting | Display | Waveshare `04_gfx_helloworld` |
| Wi-Fi signal explorer | Wi-Fi, display | Waveshare `05_esp_wifi_analyzer` |
| Tilt readings on screen | Motion sensor, display | Waveshare `03_qmi8658_example` plus a display example |
| Physical-button counter | Buttons, display | Waveshare `02_button_example` plus a display example |

The starting-point names refer to **manufacturer examples**, not files provided by this repository.

## Playful standalone projects

| Idea | Uses | First achievable version |
| --- | --- | --- |
| Magic 8-Ball or shake-to-roll dice | Motion, display | Shake detection and one random answer |
| Focus timer | Display, touch, speaker | Countdown plus a simple alert |
| Reaction-time game | Display, touch | Tap after a signal and show elapsed time |
| Tiny virtual pet | Display, touch, motion | Three facial expressions and one interaction |
| Tilt maze | Motion, display | Move a dot or ball around the screen |
| Sound visualizer | Microphones, display | One changing bar or meter |

## Connected and ambitious projects

| Idea | Uses | Added considerations |
| --- | --- | --- |
| Weather or API dashboard | Wi-Fi, display | Choose an available API; avoid exposing secrets in firmware |
| Computer status screen | Wi-Fi, display | Companion application or local API |
| BLE controller | Bluetooth LE, buttons/touch | Compatible receiver and protocol |
| Voice-controlled companion | Microphones, speaker, display | Audio handling; offline command recognition or external services |
| Conversational desk character | Audio, display, Wi-Fi | External AI service and credential handling |

A microSD card may help for larger media assets and recordings but is not required for the basic display, motion, touch, or Wi-Fi ideas.

## If you're using a coding assistant

Give it the **exact board model**, a link to [Waveshare's documentation](https://docs.waveshare.com/ESP32-S3-Touch-LCD-1.54), and a small desired behavior. Ask it to identify which existing manufacturer example is the closest starting point, explain what it will change, and propose a way to verify the result. Inspect the changes before flashing.

You can also start without AI, or use it only to help understand unfamiliar code.

## Share a discovery

An interesting result can be a working application, a failed experiment with an explanation, or an improved setup instruction. When contributing, distinguish **tried on hardware** from **not yet tested**.
