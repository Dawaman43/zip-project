# zip-project

Interactive CLI tool to zip project directories, excluding `node_modules`, `.git`, and other build/artifacts folders while preserving `.env` and other hidden config files.

## Features

- Interactive directory selection (uses fzf if available)
- Excludes `node_modules`, `.git`, `__pycache__`, `.venv`, `venv`, `.pytest_cache`, `dist`, `build`, `.next`, `.nuxt`, `target`, `vendor` at any depth
- Preserves `.env` and all hidden config files
- Shows excluded directory counts before confirming
- Saves to `~/Documents/zip-files/{project-name}.zip`

## Usage

```bash
zip-project
```

## Installation

```bash
git clone https://github.com/dawaman43/zip-project.git
cd zip-project
chmod +x zip-project
sudo ln -s "$(pwd)/zip-project" /usr/local/bin/zip-project
```

## Requirements

- `zip` command (`sudo apt install zip` on Ubuntu/Debian)
- `fzf` (optional, for interactive selection)
