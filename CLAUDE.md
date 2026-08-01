# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project purpose

This repository is Benjamin's personal research workspace supporting his PhD research on **explainability and internal mechanisms of language models**. It's used for experimenting with:

- Large Language Models (LLMs), embeddings, and encoder models
- Explainable AI (XAI) / interpretability
- Bibliometrics
- NLP

Concretely, the work here consists of:
- Running experiments in Python with transformer and embedding models
- Analyzing papers and datasets related to LLM/NLP interpretability
- Jupyter notebooks, scripts, and research notes
- LaTeX sources for papers and presentations

## Current state

The repository is in its initial, pre-code stage (empty `README.md`, no source files yet). There are no build/lint/test commands to run because no manifests or code exist yet. The sections below are the intended stack and conventions to follow as the repo grows — update this file with real commands once dependency manifests exist.

## Planned stack

- Python, managed with **uv** (not pip/conda/poetry directly) — use `uv venv`, `uv add <package>`, `uv run <command>` once a `pyproject.toml` exists
- PyTorch
- Hugging Face Transformers
- Sentence Transformers
- Jupyter notebooks
- LaTeX, for papers and presentations

## Conventions

- Keep notebooks in `notebooks/`.
- Keep reusable code in `src/`.
- Keep data separated from code (don't mix datasets into `src/` or `notebooks/`).
- Prefer reproducible experiments (pin seeds/versions, avoid hidden state/manual steps).
- Explain significant changes before modifying files — don't make large edits silently.
- Avoid creating unnecessary architecture/abstractions before the project's needs are understood — this is research code; favor simplicity over premature structure.
