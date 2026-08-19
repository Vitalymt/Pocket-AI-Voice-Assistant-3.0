# Pocket AI Voice Assistant 3.0

**Pocket-sized AI assistant. Speak — it responds.**

A tiny robot from the future that fits in your palm. ESP32-S3, 1.3" OLED display, magnetic charging, zero physical buttons.

<img src="assets/bips-v3.jpg" width="400"/>

---

## What's New in v3.0

Compared to [v1](https://github.com/Vitalymt/Pocket-AI-Voice-Assistant) and [v2](https://github.com/Vitalymt/Pocket-AI-Voice-Assistant-2.0):

- **Bigger screen** — 1.3" SH1106 OLED (was 0.96" SSD1306)
- **Zero physical buttons** — capacitive touch button hidden inside the case, responds to touch through the plastic. Acts as both "speak" and "wake from sleep"
- **Magnetic charging** — pogo pins replace dual USB-C connectors. Like wireless earbuds: drop it on the charger and it charges
- **43x43mm body** — thinner, fewer holes (only the speaker opening)
- **Better speaker** — cleaner sound, louder voice output
- **Smart sleep** — screen off after 2 minutes, deep sleep after 5 minutes. Wakes on touch
- **Web search** — Tavily API, searches the internet and responds with voice
- **OTA updates** — firmware updates over the air, no cables needed

## Specs

- **Brain:** ESP32-S3 N16R8 (16MB flash, 8MB PSRAM)
- **Board:** XH-S3E-AI V1.0 (audio amplifier built-in)
- **Display:** SH1106 1.3" OLED, 128x64, I2C
- **Audio:** I2S, 16kHz, speaker + microphone
- **Body:** 43x43mm, thin, minimal openings
- **Button:** capacitive TTP223 inside the case (touch through plastic)
- **Charging:** magnetic via pogo pins
- **Battery:** LiPo
- **Wi-Fi:** 802.11 b/g/n
- **Language:** Russian

## How It Works

1. **Touch** — the device wakes up
2. **Speak** — the microphone records your voice
3. **Think** — speech goes to the cloud, AI processes it
4. **Respond** — the speaker plays the answer
5. **Silent for 2 minutes** — screen turns off
6. **Silent for 5 minutes** — deep sleep, wakes on touch

## Components

- **Board:** XH-S3E-AI V1.0 (ESP32-S3 N16R8 + built-in audio amplifier)
- **Display:** SH1106 1.3" OLED (I2C, 128x64)
- **Microphone:** INMP441 (I2S)
- **Button:** TTP223 (capacitive, inside the case)
- **Battery:** LiPo
- **Charging:** magnetic, pogo pins

## Pinout

**Display SH1106:**
- SDA — GPIO41
- SCL — GPIO42

**Speaker (I2S, built into board):**
- DOUT — GPIO7
- BCLK — GPIO15
- LRCK — GPIO16

**Microphone INMP441:**
- SCK — GPIO5
- WS — GPIO4
- DIN — GPIO6

**Touch button TTP223:**
- SIG — GPIO43

**Volume buttons:**
- VOL+ — GPIO40
- VOL- — GPIO39

**LED:** GPIO48

## Generations

- [v1](https://github.com/Vitalymt/Pocket-AI-Voice-Assistant) — first generation, 0.96" OLED, dual USB-C, physical toggle switch
- [v2](https://github.com/Vitalymt/Pocket-AI-Voice-Assistant-2.0) — transparent case, touch button, 4 LED battery indicator
- **v3** — you are here. 1.3" OLED, magnetic charging, zero physical buttons

## Contact

- Telegram: [@hitdata](https://t.me/hitdata)
