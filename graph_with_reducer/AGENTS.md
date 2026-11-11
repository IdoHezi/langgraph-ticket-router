# Folder Guidelines

## Purpose

This folder contains Google Colab examples for LangGraph graphs that use reducers. Keep notebooks and supporting Python files here, organized by example or concept.

## Development

- Write Python compatible with the standard Google Colab runtime where practical.
- Keep notebook cells focused, ordered, and runnable from top to bottom in a fresh runtime.
- Include setup cells for nonstandard dependencies and concise Markdown explaining inputs and outputs.
- Use four-space indentation, descriptive `snake_case` names, and `PascalCase` class names.
- Avoid hidden state and values that depend on cells being run out of order.

## Verification

Run notebooks from a fresh Colab runtime before sharing. For supporting Python modules, use `python -m compileall <path>` for syntax checks and `python -m pytest` when tests are present. Document required runtime settings or Colab secrets without including secret values.

## Security

Do not commit credentials, secret values, or private datasets. Validate external input at system boundaries.
