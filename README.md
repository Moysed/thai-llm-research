# Thai LLM Research

A build-vs-buy analysis of open-source Thai LLMs (Typhoon, OpenThaiGPT, Pathumma, SEA-LION) for replacing Gemini/GPT in a Thai English-learning app — May 2026.

📄 **Read online**: [English](https://moysed.github.io/thai-llm-research/en.html) · [ภาษาไทย](https://moysed.github.io/thai-llm-research/th.html)

📊 **Bench report (2026-05-08)**: [English](https://moysed.github.io/thai-llm-research/bench-2026-05-08.html) · [ภาษาไทย](https://moysed.github.io/thai-llm-research/bench-2026-05-08-th.html) — Typhoon 2.5 vs Gemini Flash-Lite head-to-head + Round 2 with all 4 sovereign ThaiLLM Playground 8B models (KBTG, AIEAT, SCB 10X, NECTEC).

## What's inside

- **Workload analysis** — how the app actually uses LLMs (prompt size, latency budget, schema)
- **Top 3 candidates** — Typhoon (winner), OpenThaiGPT, Pathumma — with size variants, license terms, benchmarks
- **Comparison matrix** — 9 models scored across params, license, function-calling, Thai benchmarks
- **Self-hosting economics** — break-even point of hosted API vs self-host, GPU rental tiers
- **Production stack** — LiteLLM (routing) + vLLM (serving), with example configs
- **4-phase rollout plan** — from zero-GPU LiteLLM gateway → self-hosted Typhoon-12B
- **Gotchas** — quantization sensitivity for Thai, license caps, code-switching, tokenizer efficiency

## Files

| File | Purpose |
|------|---------|
| `index.html` | Landing page, auto-redirects Thai browsers to `th.html` |
| `en.html` | English version (~29 KB) |
| `th.html` | Thai version (~62 KB, more detailed) |
| `bench-2026-05-08.html` | Head-to-head bench report (English) — Round 1 Typhoon vs Gemini, Round 2 sovereign ThaiLLM 8B × 4 |
| `bench-2026-05-08-th.html` | รายงาน Bench (ภาษาไทย) — เนื้อหาเดียวกัน แปลและเรียบเรียงเป็นไทย |

All single-file, no JS dependencies, mobile-responsive, dark-mode aware, print-friendly.

## License

Research content: CC-BY-4.0. Cite if you reuse.
