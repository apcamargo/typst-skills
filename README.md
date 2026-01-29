# Typst agent skills

This repository contains a collection of agent skills for writing, editing, and debuging [Typst](https://typst.app) documents.

Most models struggle with Typst syntax since it's relatively new compared to LaTeX. These skills solve that by including local copies of documentation, examples, and specialized prompts. Instead of hallucinating syntax or guessing based on outdated training data, the agent is instructed to search through these local resources to find the correct functions and parameters before writing code.

## Available skills

### [typst-author](./typst-author/)
The general-purpose skill for writing Typst documents. It includes a complete mirror of the official Typst documentation (references, tutorials, and guides).

### [touying-author](./touying-author/)
A specialized skill for creating presentation slides using the [Touying](https://github.com/touying-typ/touying) package. It includes a full local copy of the Touying documentation, along with examples for creating slide decks, animations, and custom themes.

## Usage

If you are using an agent that supports the [Agent Skills](https://agentskills.io/home) open standard:

1. Clone this repository.
2. Move or copy the individual skill directories (`typst-author`, `touying-author`) into the `skills/` folder of your agentic coding assistant.

The agent should automatically detect the skills and use them whenever you ask for help with Typst files or Touying presentation slides.
