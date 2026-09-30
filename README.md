# ocrlook

**Extract structured JSON from images and PDFs using AI — right in your browser.**

ocrlook lets you upload an image or PDF, optionally define the fields you want, and get clean JSON back.  
API keys stay in your browser. No server. No account.

---

## Features

- **Image & PDF support** — PDFs are rendered to high-quality images using PDF.js
- **Multi-provider AI** — OpenRouter, OpenAI, Google Gemini, Anthropic Claude, DeepSeek
- **Schema-based extraction** — Provide keys and get exact matching JSON
- **Auto mode** — No schema? Get line-by-line extraction (`line_1`, `line_2`, ...)
- **Custom instructions** — Guide the AI with extra rules (date formats, ignore notes, etc.)
- **Local storage** — API keys are saved only in your browser
- **Zero backend** — Pure HTML, CSS, and JavaScript

---

## How it works

1. Select your AI provider and paste the API key
2. (Optional) Enter the fields you want to extract
3. (Optional) Add custom instructions for the AI
4. Upload an image or PDF
5. Click **Extract JSON**

For PDFs, ocrlook renders the selected page to an image first, then sends that image to the vision model.

---

## Supported Providers

| Provider       | Notes                              |
|----------------|------------------------------------|
| OpenRouter     | Recommended — access many models   |
| OpenAI         | GPT-4o                             |
| Google Gemini  | Gemini 2.0 Flash                   |
| Anthropic      | Claude 3.5 Sonnet                  |
| DeepSeek       | Limited vision support             |

---

## Usage

1. Download or clone this repository
2. Open `index.html` in any modern browser
3. Add your API key and start extracting

No build step. No installation.

---

## Privacy

- All processing happens in your browser
- API keys are stored in `localStorage` only
- Images and PDFs are never uploaded to any ocrlook server
- Only the selected AI provider receives the image data

---

## Tech Stack

- HTML, CSS, JavaScript
- [PDF.js](https://mozilla.github.io/pdf.js/) for PDF rendering
- Direct API calls to vision models

---

## License

MIT
