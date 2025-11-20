# simple-chatgpt

Simple command-line tool to use ChatGPT Desktop from your Mac terminal.

Behind the scenes it forwards your input to a macOS Shortcut included with the install. No OpenAI API key required.

## Install

```bash
brew tap paolofulgoni/simple-chatgpt https://github.com/paolofulgoni/simple-chatgpt
# Until a release is tagged, install from HEAD:
brew install --HEAD paolofulgoni/simple-chatgpt/simple-chatgpt
# Import the Shortcut into the Shortcuts app:
open "$(brew --prefix)/share/simple-chatgpt/simple-chatgpt.shortcut"
```

Requires ChatGPT Desktop to be installed on your Mac.

On first run, Shortcuts will ask to “Allow ‘simple-chatgpt’ to share 1 text item with ‘ChatGPT’?”. Click **Always Allow**.

The included Shortcut uses the standard “Run ChatGPT” action shipped with the ChatGPT Desktop app: no hacks or custom integrations.

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
simple-chatgpt -o answer.txt "What does 'anolini' mean?"
```

Get help:

```bash
simple-chatgpt -h
```

## Disclaimer

ChatGPT is a product and trademark of OpenAI. This utility is not affiliated with or endorsed by OpenAI.
