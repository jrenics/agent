# README for the agent repository

## Objective

This repository contains notes and changes I created during my exploration of agents. 
It focuses on insights and learnings.

I will directly update this doc. Once a note is mature enough I will separate it out to its own md file.

## Content

My first goal is to run a local coding agent that can help producing insightful code and doc, not just useful/runnable stuff.

### Hardware Setup

### Model: Qwen 3.8 27B

Because it is even better than Opus 4.6, according to Artificial Analysis. And it fits into my hardware.

### Harness: Claude Code, Codex, Qwen Code

Because claude code made a big impact in harness cli, codex is open sourced from the other company, and qwen code is native with qwen model.

### Serving Stack

#### Llama.cpp

#### vllm

#### Ollama

### Benchmark Task 1: Produce a Book

Issues:
  - The current agent/harness cannot run without human intervention in the current setup.
  - The speed is limited, but this might be inevitable with the current hardware.
  - Llama.cpp has issue with the CUDA in my hardware
  - Claude Code needs litellm to use Qwen as its auto mode classifier
  - Local codex does not have a usable web search tool
  - Local codex or qwen code does not show version number