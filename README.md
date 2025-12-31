# typst-author skill

`typst-author` is an agent skill that guide AI agents to write [Typst](https://typst.app/docs/).

Most models struggle with Typst syntax since it's relatively new compared to LaTeX. This repo solves that by including a local copy of the entire documentation (references, tutorials, and guides) in the `docs/` directory. Instead of hallucinating syntax or guessing based on outdated training data, the agent is instructed to search through these local docs to find the correct functions and parameters before writing code.

## What's Inside

- [**`SKILL.md`**](./SKILL.md): The system prompt that tells the agent how to use this repository.
- [**`docs/`**](./docs/): A complete mirror of the official Typst documentation.

## Usage

If you are using an agent that supports the [Agent Skills](https://agentskills.io/home) open standard, just clone this repository and place it in the skills folder of your agentic coding assistant. Agents should automatically detect the `typst-author` skill and use it whenever you ask for help with Typst files.
