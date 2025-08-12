---
id: cheatsheet1-ollama-cli
title: Ollama CLI Essentials - Cheatsheet Style
sidebar_position: 1
description: Concise Ollama CLI reference with commands and usage.
---

# Ollama CLI Essentials

| Command                      | Description, Usage & Example                                                                                             |
|------------------------------|-------------------------------------------------------------------------------------------------------------------------|
| **`ollama --version`**        | **What:** Show installed Ollama CLI version.<br />**Why:** Verify version and troubleshoot.<br />**How:** `ollama --version`<br />**Example:** `ollama version 1.2.3` |
| **`ollama list`**             | **What:** List installed models.<br />**Why:** Manage models and disk space.<br />**How:** `ollama list`<br />**Example:**<br />> llama2:7b (installed)<br />> mymodel (installed) |
| **`ollama pull <model>`**     | **What:** Download model locally.<br />**Why:** Required before use.<br />**How:** `ollama pull llama2:7b`<br />**Example:**<br />> Downloading llama2:7b...<br />> Done. |
| **`ollama run <model> -p "<prompt>"`** | **What:** Run inline prompt.<br />**Why:** Quick interaction.<br />**How:** `ollama run llama2:7b -p "Write a haiku"`<br />**Example:**<br />> Autumn leaves falling<br />> Soft whispers in the breeze<br />> Nature's quiet song |
| **`ollama run <model> -f <file>`** | **What:** Run prompt from file.<br />**Why:** Manage complex prompts.<br />**How:** `ollama run llama2:7b -f prompt.txt`<br />**Example:**<br />File `prompt.txt` contains: `Write a haiku about autumn`<br />Output:<br />> Autumn leaves falling<br />> Soft whispers in the breeze<br />> Nature's quiet song |
| **`ollama create <model>`**   | **What:** Create custom model.<br />**Why:** Customize & fine-tune.<br />**How:** `ollama create mymodel -f Modelfile`<br />**Example:** `Model "mymodel" created successfully.` |
| **`ollama delete <model>`**   | **What:** Delete local model.<br />**Why:** Free disk space.<br />**How:** `ollama delete llama2:7b`<br />**Example:** `Deleted model llama2:7b.` |

---

## Pro Tips

- Always pull before running new models.  
- Use `-p` for short prompts, `-f` for longer prompts.  
- Run `ollama list` regularly to clean up unused models.
```

---

**To use:**

* Save this text as `ollama-cli-essentials.md` (or any `.md` file)
* Add it to your Docusaurus `/docs` folder or your markdown repo
* It will render as a clean, easy-to-read cheat sheet with proper line breaks and formatting

