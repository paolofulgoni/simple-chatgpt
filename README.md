# simple-chatgpt

Command-line access to ChatGPT on macOS via a Shortcuts workflow.

## Install

```bash
brew tap paolofulgoni/simple-chatgpt https://github.com/paolofulgoni/simple-chatgpt
# Until a release is tagged, install from HEAD:
brew install --HEAD paolofulgoni/simple-chatgpt/simple-chatgpt
# Import the Shortcut into the Shortcuts app:
open "$(brew --prefix)/share/simple-chatgpt/simple-chatgpt.shortcut"
```

On first run, Shortcuts will ask something like “Allow ‘simple-chatgpt’ to share 1 text item with ‘ChatGPT’?”. Click **Always Allow**.

## Use

Ask a question directly:

```bash
simple-chatgpt "What is the capital of Italy?"
```

Read a prompt from a file:

```bash
simple-chatgpt -f prompt.txt
```

Write the answer to a file:

```bash
simple-chatgpt "What does 'anolini' mean?" -o answer.txt
```

Get help:

```bash
simple-chatgpt -h
```
