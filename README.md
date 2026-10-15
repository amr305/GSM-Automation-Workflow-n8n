# GSM Marketing & Lead Acquisition Automation Pipeline (n8n + AI)

An end-to-end automated workflow built with **n8n** that integrates digital marketing lead capture, real-time market research, local multimodal AI generation, automated video rendering, and multi-channel notification.

## 🛠️ Architecture & Workflow Zones
1. **Zone 1: Ingestion & Lead Capture:** Captures lead entries via Google Forms/Sheets integrated with Facebook & LinkedIn ads.
2. **Zone 2: Live Market Research:** Queries DuckDuckGo for live pricing, metrics, and market data.
3. **Zone 3: Local AI Generation:** Uses Ollama (LLaVA) locally for script generation, offer creation, and analysis without external API costs.
4. **Zone 4: Automated Video Engine (MoneyPrinterTurbo):** Orchestrates local **MoneyPrinterTurbo** rendering, utilizing **ElevenLabs TTS** (voice synthesis), **Pixabay b-roll footage**, and **FFmpeg subtitle animation** to compose final personalized video assets via sub-workflow.
5. **Zone 5: Multi-Channel Outreach:** Dispatches custom proposals via Email and sends real-time lead alerts through Telegram bots (or any channel supported by n8n).

## 📂 Repository Contents
- `Main workflow .json`: The core n8n automation pipeline.
- `My video workflow .json`: Sub-workflow triggering MoneyPrinterTurbo rendering and media stitching.
- `automation workflow.jpeg`: High-resolution architecture canvas map.

## 🚀 How to Import
1. Download both JSON files (`Main workflow .json` and `My video workflow .json`).
2. Open your n8n instance.
3. Import both workflows (`Workflows` -> `Import from File`).
4. Ensure the video generation node references MoneyPrinterTurbo and the imported sub-workflow.
