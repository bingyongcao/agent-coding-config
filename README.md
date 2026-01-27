# Agent Coding Config

A centralized configuration repository for the Antigravity agent. This project defines the global rules, specialized skills, and automated workflows that guide the agent's behavior, ensuring consistent code quality and uniform project structures across user workspaces.

## Features

### 🧠 Skills
Specialized capabilities that extend the agent's toolkit:
- **Creating Skills** (`skills/creating-skills`): Standards and templates for generating new agent skills, ensuring they follow the "Antigravity" structural requirements.
- **Creating Workflows** (`skills/creating-workflows`): Guidelines for defining robust, step-by-step automation workflows (turbo mode, step validation).

### ⚡ Workflows
Automated sequences of tasks to speed up development:
- **Generate README** (`/generate-readme`): Automatically analyzes a codebase and generates a comprehensive `README.md` file (like this one!).

### 📏 Global Rules
- **Code Style**: Enforces naming conventions (PascalCase for classes, camelCase for local vars) and formatting (Allman braces).
- **Architecture**: Promotes patterns like Repository, Dependency Injection, and Single Responsibility.
- **Performance & Quality**: Guidelines for optimization and robust error handling.

## Project Structure

```
├── .agent/
│   └── workflows/       # Workflow definitions (.md)
├── rules/               # Global rule definitions
├── skills/              # Skill definitions and resources
└── README.md            # Project documentation
```

## Usage

This repository is intended to be loaded by the Antigravity agent as a configuration source.
1. **Clone** this repository to your local machine.
2. **Configure** your agent setting to point to this directory (or specific files within it) as the source of truth for rules and skills.

## Contributing

- **New Skills**: Create a new folder in `skills/` defined by `SKILL.md`.
- **New Workflows**: Add `.md` files to `.agent/workflows/` with valid YAML frontmatter.
