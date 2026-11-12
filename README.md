# Anatomy of a Chatbot

An interactive, single-file website that explains how LLM chatbots such as ChatGPT, Claude and Grok work, from the moment you type a message to the moment the answer streams back.

## Overview

Most explanations of LLMs are either too shallow or buried in papers. This project walks through the full pipeline with live, hands-on demos, and ends with an honest look at where quantum computing fits (and doesn't).

## Features

- **Live tokenizer:** type a sentence and watch it split into tokens with IDs (simplified demo tokenizer).
- **Nine-stage pipeline:** tokenization, embeddings, self-attention, transformer blocks, logits and softmax, sampling, the generation loop with KV cache, training, and serving with tools. Each stage includes key points and the underlying formula or pseudocode.
- **Attention visualizer:** select a word to see weighted arcs to the words it attends to, with a causal-mask toggle.
- **Temperature and sampling lab:** a slider reshapes the softmax distribution in real time, and you can sample tokens from it.
- **Autoregressive loop animation:** shows one forward pass per token and the KV cache growing.
- **Quantum computing section:** a single-qubit rotation and measurement demo, plus an exponential-amplitude counter that shows why scale is the hard part.
- **Model comparison:** ChatGPT, Claude and Grok, limited to publicly documented details.

## Tech stack

- HTML, CSS and vanilla JavaScript in one file, with no build step and no dependencies
- Google Fonts: Instrument Serif and Hanken Grotesk, with system fallbacks
- Inline SVG for the attention arcs
- Respects `prefers-reduced-motion` and is responsive down to mobile

## Run locally

```bash
git clone https://github.com/hammadhafee55/anatomy-of-a-chatbot.git
cd anatomy-of-a-chatbot
# open index.html in any browser
```

## Deploy on GitHub Pages

1. Rename `chatbot-anatomy.html` to `index.html`.
2. Go to **Settings → Pages**.
3. Set the source to the `main` branch and the `/ (root)` folder, then save.

## Accuracy notes

- Token IDs, attention weights and logits in the demos are illustrative, not taken from a real model.
- Details of the newest proprietary models are not public, so the comparison table covers only what each company has described.

## Author

**Muhammad Hammad Hafeez**, Data Scientist, ML Expert and Data Analyst

- LinkedIn: https://www.linkedin.com/in/muhammad-hammad-hafeez-03945023b
- GitHub: [@hammadhafee55](https://github.com/hammadhafee55)
- Contact: +92 347 6730754

Built under **[Nexoritha](https://hammadhafee55.github.io/Nexoritha/)**, a company delivering data analytics, AI/ML and digital services.

## License

MIT License. See `LICENSE` for details.
