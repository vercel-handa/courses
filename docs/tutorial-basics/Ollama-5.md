
---

## Ollama Chat & Interaction Commands

<details>
<summary><code>ollama chat &lt;model&gt;</code></summary>

**What:** Start an interactive chat session with the model.<br />
**Why:** Allows continuous conversational interaction.<br />
**How:** Run this command with model name.<br />

**Example:**

```shell
ollama chat llama2
```

</details>

<details>
<summary><code>--history &lt;file&gt;</code></summary>

**What:** Loads chat history from a file.<br />
**Why:** Maintain context over multiple sessions.<br />
**How:** Pass history file when starting chat.<br />

**Example:**

```shell
ollama chat llama2 --history chat_history.json
```

</details>

<details>
<summary><code>--no-history</code></summary>

**What:** Runs chat without saving or loading history.<br />
**Why:** Use for one-off chats without persistent context.<br />
**How:** Add this flag to chat command.<br />

**Example:**

```shell
ollama chat llama2 --no-history
```

</details>

<details>
<summary><code>--system &lt;string&gt;</code></summary>

**What:** Overrides the system prompt for the chat session.<br />
**Why:** Change assistant’s behavior or personality.<br />
**How:** Provide system prompt string.<br />

**Example:**

```shell
ollama chat llama2 --system "You are a helpful assistant."
```

</details>

<details>
<summary><code>--max-tokens &lt;number&gt;</code></summary>

**What:** Limits maximum tokens per response.<br />
**Why:** Control response length.<br />
**How:** Add this flag with desired number.<br />

**Example:**

```shell
ollama chat llama2 --max-tokens 150
```

</details>

