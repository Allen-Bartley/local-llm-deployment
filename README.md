# 🧠 Local LLM Deployment on *Rose Red*

## Overview

This repository documents the installation, configuration, and experimentation with locally run language models using LM Studio and Ollama on a custom Windows 11 desktop named **Rose Red**. It blends technical reproducibility with philosophical inquiry, focusing on autonomous AI behavior, prompt freedom, and offline persona modeling.

## 🖥️ System Specs

| Component       | Details |
|----------------|---------|
| OS             | Windows 11 Pro 64-bit |
| CPU            | Intel Core i7-12700K (Alder Lake, 10nm) |
| RAM            | 32 GB **DDR5** @ 5600 MHz (Corsair VENGEANCE CL36) |
| GPU            | NVIDIA RTX 3060 (12GB) |
| Storage        | ~25TB across internal and USB drives |
| Displays       | Sceptre F27 (3840×2160 @ 100Hz), HP 27mq (3620×2036 @ 59Hz) |
| Audio          | Realtek High Definition Audio |

## 📦 Installed Models

### LM Studio v0.3.16

| Model Name                                             | Architecture | Params | Quantization | Size    | Purpose                           |
|--------------------------------------------------------|--------------|--------|--------------|---------|-----------------------------------|
| writing-roleplay-20k-context-nemo-12b-v1.0             | llama        | 12B    | Q4_K_S        | 7.12 GB | Longform persona-driven writing   |
| nemo-12b-humanize-kto-v0.1                             | llama        | 12B    | Q4_K_S        | 7.12 GB | Humanized conversational agent    |
| pocketdoc_dans-personalityengine-v1.3.0-24b            | llama        | 24B    | Q4_K_S        | 13.55 GB| Complex character emulation       |
| llama-3.1-8b-lexi-uncensored-v2                        | llama        | 8B     | Q4            | 4.66 GB | Unfiltered model interaction      |
| deepseek-r1-distill-qwen-14b                          | qwen2        | 14B    | Q4_K_M        | 8.99 GB | Logic-driven summarization        |
| meta-llama-3.1-8b-instruct                            | llama        | 8B     | Q4_K_M        | 4.92 GB | Instruction-following tasks       |
| gemma-2-9b-it                                         | gemma2       | 9B     | Q4_K_M        | 5.76 GB | Clean, technical communication    |
| llama-3.2-1b-instruct                                 | llama        | 1B     | Q8            | 1.32 GB | Lightweight testing & debugging   |

> LM Studio Total Footprint: ~58.5 GB

### Ollama CLI

Use `ollama list` and `ollama show <model>` to view installed models and their metadata.

| Model Name       | Params | Size   | Purpose                            |
|------------------|--------|--------|------------------------------------|
| qwen2.5:14b       | 14B    | ~9.0GB | Uncensored philosophical dialog    |
| deepseek-r1:14b   | 14B    | ~9.0GB | Structured logical inference       |

## ⚙️ Installation Summary

- **LM Studio:** Installed via official Windows `.exe` installer
- **Ollama:** Installed via CLI following an online step-by-step guide
- **Model Formats:** GGUF for LM Studio; Ollama uses proprietary backend
- **Inference Mode:** CPU + GPU acceleration enabled (RTX 3060 leveraged)

## 🧪 Use Cases

- Testing uncensored LLM behavior in air-gapped environments
- Persona creation and RPG character emulation
- Prompt engineering, tone modeling, and jailbreaking workflows
- Summarization using grounded personal source material
- Philosophical dialog experiments without content filtering

## 🎯 Philosophy

> “Cloud models are polite. Local models tell stories the way *you* want.”

This setup reflects a broader mission: investigating how autonomous models behave when freed from corporate filters, and how custom context injection reshapes AI reasoning. Inspired by the resilience and complexity found in *Fallout: Equestria* and *Project Horizons*, this project treats local language models as both ethical tools and narrative mirrors.

## 🔧 Planned Modules

- `context-injection/`: Markdown and PDF grounding experiments
- `persona-scripts/`: Chat flows for fictional agents and RPG testing
- `prompt-gallery/`: Prompt comparisons across model behavior
- `benchmark-results/`: Token speed, memory usage, and inference fidelity

---

*This repo will evolve alongside the Rose Red build and future explorations in autonomous storytelling, ethical tooling, and hybrid compute development.*

