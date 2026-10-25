# ✨ Nova — Voice + AI Command Automation Agent

Soft-themed chat agent that runs **100% in the browser**. Type or speak a command; Nova plans, picks tools, executes. **No API keys, no backend, no cost.**

## Features
- 🎤 **Voice commands** (Web Speech API) with spoken replies
- 🧠 **AI mode**: an LLM running inside your browser (WebLLM + WebGPU) turns natural language / Hinglish into tool calls
- ⛓ **Multi-step chaining**: `add task study and then timer 30 sec and then joke`
- Tasks, notes, timers, calculator, password generator, open sites, Google/YouTube search, live weather, Wikipedia
- Light/dark mode, pastel glassmorphism UI

## Architecture
`Voice/Text → (optional LLM planner) → Intent router → Async tools → Chat output (+ speech)`
Add a tool by adding one object (`re` + `run`) to the `tools` array in `index.html`.

## Run
- Online: GitHub Pages link (recommended, HTTPS needed for mic + AI)
- Local: `python -m http.server 8000` then open http://localhost:8000

## Browser support
Voice: Chrome / Edge. AI mode: desktop Chrome / Edge with WebGPU (first load downloads the model, then cached).

Built by [contentbyshanu](https://linkedin.com/in/contentbyshanu)
