
---

## Ollama Configuration & Environment Variables

<details>
<summary><code>OLLAMA_API_KEY</code></summary>

**What:** Environment variable for your Ollama API key.<br />
**Why:** Authenticate requests securely.<br />
**How:** Set it in your shell or environment before using Ollama CLI or SDK.<br />

**Example:**

```bash
export OLLAMA_API_KEY="your_api_key_here"
```

</details>

<details>
<summary><code>OLLAMA_HOST</code></summary>

**What:** Sets custom Ollama host endpoint.<br />
**Why:** Useful if running Ollama on a different server.<br />
**How:** Set environment variable accordingly.<br />

**Example:**

```bash
export OLLAMA_HOST="http://localhost:11434"
```

</details>

<details>
<summary><code>OLLAMA_MODEL_PATH</code></summary>

**What:** Overrides default path to local models.<br />
**Why:** Useful if you store models in a custom location.<br />
**How:** Set environment variable.<br />

**Example:**

```bash
export OLLAMA_MODEL_PATH="/custom/models/path"
```

</details>

<details>
<summary><code>OLLAMA_LOG_LEVEL</code></summary>

**What:** Sets the logging verbosity.<br />
**Why:** Debug or reduce log output.<br />
**How:** Set one of: DEBUG, INFO, WARN, ERROR.<br />

**Example:**

```bash
export OLLAMA_LOG_LEVEL="DEBUG"
```

</details>

<details>
<summary><code>config.yaml</code></summary>

**What:** Ollama config file to set default CLI options.<br />
**Why:** Avoid specifying flags every time.<br />
**How:** Create `config.yaml` in your home or project directory.<br />

**Example:**

```yaml
default_model: llama2
temperature: 0.7
max_tokens: 200
```

</details>

