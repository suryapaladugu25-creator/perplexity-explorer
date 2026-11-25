# 🚀 Perplexity Explorer — Comic AI Adventure

An interactive, comic-book-style educational game that demonstrates how large language models (LLMs) calculate perplexity, token probabilities, and next-token predictions in real time.

Built with **vanilla HTML, CSS, and modern JavaScript**, powered by **Transformers.js v3** and the real quantized **DistilGPT-2** language model running 100% locally in the browser via WebAssembly/WebGPU.

---

## 🎮 Features & Missions

- **Mission 01 — Decode the Sentence:** Type or choose sample sentences to calculate real cross-entropy loss, bits per token, and perplexity with animated futuristic scanning.
- **Mission 02 — Token Detective:** Inspect each token's conditional probability $P(w_i \mid w_{<i})$, reciprocal surprise ratio ($1/P$), and surprise level in bits ($-\log_2 P$).
- **Mission 03 — Prediction Arena:** Top 8 next-token predictions from DistilGPT-2 logits with interactive token appending.
- **Mission 04 — Perplexity Lab (Simulator):** Interactive theoretical probability sandbox with sliders, real-time formula breakdowns, and live perplexity calculation.
- **BYTE-01 Robot Mascot:** Illustrated cartoon AI guide with speech bubble commentary and interactive tips.
- **Gamification & XP:** Track Explorer Level, earn XP, complete missions, and unlock 6 achievement badges persisted via `localStorage`.
- **Sound Effects:** Synthesized retro arcade audio using the Web Audio API (disabled by default, togglable anytime).
- **Comic Intel Lore:** 4-panel dialogue explainers for Tokens, Softmax Probability, Cross-Entropy, and Perplexity.

---

## 🛠️ Local Development & Deployment

This project is a zero-build, static application centered in `index.html`.

### Run Locally

Because modern ES modules use Web Workers and WASM, serve over HTTP:

```bash
# Python 3
python3 -m http.server 3000

# Or Node.js
npx serve .
```

Then open `http://localhost:3000` in any modern web browser.

### Deploy to Vercel

1. Import this repository into your Vercel Dashboard.
2. Select **Other** as the Framework Preset (Static site).
3. Leave Build Command and Output Directory as default (`.`).
4. Deploy!
