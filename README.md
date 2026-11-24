# Replication package: Why LLM-Generated Code Fails the Way It Does

[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.24510912.svg)](https://doi.org/10.5281/zenodo.24510912)

Replication package for the paper "Why LLM-Generated Code Fails the Way It Does: A
Mechanistic Account and Its Use for Repair" by Musfiqur Rahman, Mahi Begoug and Emad Shihab
(Concordia University), submitted to ACM Transactions on Software Engineering and
Methodology (TOSEM).

> Status: work in progress. The contents below are added before submission.

The package has two parts:

1. **This repository**, archived on Zenodo at every release: code, frozen splits and
   targets, the scripts that build each table and figure, and the small result files they
   read.
2. **A data record on Zenodo** (link added at submission) for the files too large for
   GitHub: generations, per-token measures, tuned lenses, probes, directions and LoRA
   adapters.

## Layout

| Folder | Contents | Where |
|---|---|---|
| `code/` | Study code (Python package `rg5`) and cluster job scripts | here |
| `study/` | Repository list, snapshot revisions, test/dev splits, targets of the test, development and RQ4 confirmation samples, memorised-target list | here |
| `tables/` | One script per table and figure, plus the summaries they read | here |
| `prompts/` | Prompts and RQ3 context segments (RAG, CAG, KAG, oracle, noise) | data record |
| `generations/` | Generations for every model, condition and repair arm, with test outcomes | data record |
| `cases/`, `measures/` | Failing tokens, matched controls and per-token measures | data record |
| `weights/` | Tuned lenses, probes, directions, LoRA adapters | data record |

## Models

Qwen2.5-Coder-7B-Instruct, DeepSeek-Coder-6.7B-Instruct, CodeLlama-7B-Instruct,
Llama-3.1-8B-Instruct and StarCoder2-7B. Model weights are not redistributed;
`code/models.lock.json` pins the exact revisions.

## Reproducing the results

To be completed: environment setup, and one command per table or figure.

## Licence

To be completed. Only repositories whose licence allows redistribution are included.
