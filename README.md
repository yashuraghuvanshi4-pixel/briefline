# Briefline

Briefline is a privacy-first, evidence-linked meeting and document copilot designed and optimized for Snapdragon-powered HP PCs.

## Challenge submission

- **Project title:** Briefline: Private, Evidence-Linked AI Copilot for Snapdragon HP PCs
- **Primary device target:** HP PCs with Snapdragon X Elite or Snapdragon X Plus
- **AI model plan:** Whisper-Medium and Qwen3-0.6B from Qualcomm AI Hub, profiled for the target Snapdragon runtime
- **Core promise:** turn a conversation into an editable action brief while keeping audio, documents, and generated notes on the PC

## Repository contents

- `app/index.html` — runnable no-build interaction prototype with local-mode UI, evidence links, session controls, and export
- `briefline-snapdragon-proposal.html` — full proposal source
- `briefline-project-description.pdf` — upload-ready project description
- `briefline-short-pitch.html` — pitch-deck source
- `briefline-short-pitch.pdf` — upload-ready pitch PDF
- `briefline-short-pitch.pptx` — editable pitch deck
- `create_briefline_deck.py` — script used to generate the PowerPoint

## Run the prototype

Open `app/index.html` in a browser. It intentionally uses sample data so the interaction can be demonstrated immediately without pretending that the AI model assets are already bundled. The production implementation will replace the sample pipeline with Qualcomm AI Hub compiled model assets and a local runtime.

## Production implementation plan

1. Add local audio capture and chunking.
2. Deploy the AI Hub Whisper asset through the supported Snapdragon runtime.
3. Add Qwen3 structured extraction with evidence offsets.
4. Store session data in local SQLite with full-text search.
5. Profile quality, latency, memory, and battery use on the exact HP Snapdragon device.
6. Package a signed Windows installer with quality, balanced, and low-power modes.

## Submission note

The proposal labels performance numbers as targets until they are measured on the exact HP Snapdragon configuration. The participant must confirm device eligibility and ownership before submitting the challenge form.