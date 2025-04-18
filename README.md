# openweights-ai-starterkit 🤖💻

These instructions are for MacOS only at this stage. They can be easily adapted for Windows and Linux. If you would like to see instructions for Windows and/or Linux, please [open an issue ticket](https://github.com/blairwang-online/openweights-ai-starterkit/issues/new), specifying which version of Windows or which distribution of Linux. 😊

## 1. Install Homebrew 🍺

- Whilst this not strictly necessary, it will make the process much easier by automating some of the installations.
- Follow the instructions at https://brew.sh/

## 2. Install Ollama 🦙

Ollama is on GitHub: https://github.com/ollama/ollama

- If you are using Homebrew, you can simply run `brew install ollama`
- Alternatively, you can do this by directly downloading the installer from https://ollama.com/download
- Once installation is complete, you can run:
  - `ollama` (shows possible commands)
  - `ollama list` (shows installed models)
  - `ollama pull <some model>` (see https://ollama.com/search)
  - `ollama run <some model>` (chat with an AI model directly in your terminal; use `/bye` to leave)

## 3. Install Open WebUI 👨🏻‍💻

Open WebUI is on GitHub: https://github.com/open-webui/open-webui

- As per the instructions at time of writing, you will need to first install the programming language **Python 3.11**, and then use that to install Open WebUI.
- The best way to do this is using **pipx** ("Install and Run Python Applications in Isolated Environments" - see [pipx GitHub page](https://github.com/pypa/pipx))

In other words, assuming you have set up Homebrew in step 1, you just need the following commands in your terminal:

```zsh
brew install python@3.11
pip3.11 install pipx
pipx install open-webui
open-webui serve
```

Then you can just go to: http://localhost:8080
