# Gemini Live Personal Voice Assistant

This project lets you run a **real-time voice assistant** with Gemini Live using your microphone.

## Setup

1. Install dependencies:

```bash
pip install -r requirements.txt
```

2. Create a `.env` file:

```env
GEMINI_API_KEY=your_api_key_here
```

## Run

Basic voice assistant (voice-only):

```bash
python gemini-live-cam.py --mode none
```

Assistant with a custom personality:

```bash
python gemini-live-cam.py --mode none --assistant "You are my focused coding coach. Keep answers short and actionable."
```

Use camera context while speaking:

```bash
python gemini-live-cam.py --mode camera
```

Use screen context while speaking:

```bash
python gemini-live-cam.py --mode screen
```

Change speaking voice:

```bash
python gemini-live-cam.py --mode none --voice Aoede
```

Disable web search tool:

```bash
python gemini-live-cam.py --mode none --disable-search
```

## Controls

- Type messages at `message >` and press Enter to send text.
- Speak naturally; microphone audio is streamed continuously.
- Enter `q` to quit.
