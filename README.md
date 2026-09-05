# PulseGram

PulseGram is a modified Telegram client for Android based on Telegram, Nagram, and Nekogram with integrated AyuGram message saving, AI/LLM providers, and enhanced privacy features.

## Downloads

* [Telegram Channel](https://t.me/yawprod)
* [GitHub Releases](https://github.com/ANTBOLT/pulsegram/releases)

### Package Info
* Package name: `nu.gpu.nagram`
* Base version: Telegram Android v12.10.0

---

## Features

### Privacy & Ghost Mode
* **Ghost Mode**: Do not send read markers for incoming messages
* **Stories Stealth**: Do not send view receipts when watching Stories
* **Typing Status**: Hide typing and audio recording indicators
* **Online Status**: Conceal online presence
* **Local Last Seen**: Save and display local last seen timestamps

### Message & Media Saving (AyuGram)
* **Save Deleted Messages**: Retain messages deleted by other users with customizable `[deleted]` tag
* **Edit History**: Track and view message edit history
* **Media Retention**: Save self-destructing and deleted media (photos, videos, voice notes)
* **Granular Scope**: Independently configure saving in private chats, groups, and channels
* **Clear Database**: Built-in option to purge saved message history from Room DB

### AI & LLM Integration
* **Supported Providers**: OpenAI, Google Gemini (AI Studio & Vertex), Groq, DeepSeek, xAI (Grok), Cerebras, Ollama Cloud, OpenRouter, Vercel AI Gateway, and custom OpenAI-compatible endpoints
* **Context-Aware Translation**: Translates messages using chat context
* **Custom Prompts**: User-configurable system prompts and temperature settings

### Translation & Transcription
* **Nekogram Translator**: Translate text via Google, DeepL, Yandex, LibreTranslate, Lingva, or LLM
* **Formatting Preservation**: Keeps Markdown, spoilers, bold, quotes, and links intact during translation
* **Free Audio Transcription**: Speech-to-text for voice and video notes via external STT / Whisper API without Telegram Premium

### Chat & Messaging
* **Forwarding Options**: Forward messages without quotes or authors
* **Repeat as Copy**: Resend messages as direct copies
* **Text Formatting Bar**: Quick toggles and customizable ordering for bold, italic, monospace, strikethrough, underline, quote, spoiler, and link
* **Audio Enhancements**: Noise suppression and voice enhancement for voice notes
* **Double Tap Actions**: Configurable double-tap action (reply, react, translate, etc.)
* **Message Details**: Show exact message ID and precise timestamp
* **Bypass Restrictions**: Allow saving content and taking screenshots in protected chats

### Media & Player
* **Decoder Selection**: Switch between hardware and software ExoPlayer decoders
* **Playback Speed**: Fine-grained playback speed control for audio and video
* **OpenStreetMap**: Option to use OSM instead of Google Maps

### UI & Customization
* **Material You**: Dynamic Monet theme support based on system colors
* **Custom Fonts**: Support for loading external `.ttf` / `.otf` fonts
* **Custom Emoji Packs**: Support for external emoji sets
* **Interface Cleanup**: Options to hide Telegram Premium and Help sections in Settings
* **Drawer & Toolbar**: Configurable drawer items and action bar buttons

### Network & Push
* **UnifiedPush**: Full support for UnifiedPush distributors (de-Googled push notifications)
* **Custom DNS / DoH**: Built-in DNS-over-HTTPS via dnsjava
* **Proxy Automation**: Automatically disable proxy when VPN connection is active

---

## Compilation Guide

1. Clone the repository with submodules:
   ```bash
   git clone --recursive --shallow-submodules https://github.com/ANTBOLT/pulsegram.git
   cd pulsegram
   ```

2. Configure Telegram API credentials in `local.properties`:
   ```properties
   TELEGRAM_APP_ID=39680981
   TELEGRAM_APP_HASH=1295d5b2c4577850b35e8d6ffb4ca17c
   ```

3. Build with Gradle:
   ```bash
   ./gradlew TMessagesProj:assembleRelease
   ```

   *Requirements: JDK 21, Android SDK Platform 37, Build-Tools 36.0.0, NDK 27.2.12479018, CMake 3.31+, and NASM.*

Alternatively, trigger the automated **Release Build** workflow via GitHub Actions to compile in the cloud.

---

## Acknowledgments

* [Telegram for Android](https://github.com/DrKLO/Telegram)
* [Nagram](https://github.com/NextAlone/Nagram)
* [Nekogram](https://github.com/Nekogram/Nekogram)
* [AyuGram](https://github.com/AyuGram/AyuGram4A)
* [Cherrygram](https://github.com/arsLan4k1390/Cherrygram)
* [exteraGram](https://github.com/exteraSquad/exteraGram)
* [OctoGram](https://github.com/OctoGramApp/OctoGram)


