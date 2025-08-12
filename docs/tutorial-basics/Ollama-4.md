
---

## Ollama Model Management Commands

<details>
<summary><code>ollama list</code></summary>

**What:** Lists all models installed locally.<br />
**Why:** Check which models are available for use.<br />
**How:** Run this command in terminal.<br />

**Example:**

```shell
ollama list
```

</details>

<details>
<summary><code>ollama pull &lt;model&gt;</code></summary>

**What:** Downloads a model from the Ollama registry.<br />
**Why:** Required to have the model locally.<br />
**How:** Replace `<model>` with the desired model name.<br />

**Example:**

```shell
ollama pull llama2
```

</details>

<details>
<summary><code>ollama stop &lt;model&gt;</code></summary>

**What:** Stops a running model instance.<br />
**Why:** Free up system resources.<br />
**How:** Replace `<model>` with the model name.<br />

**Example:**

```shell
ollama stop llama2
```

</details>

<details>
<summary><code>ollama delete &lt;model&gt;</code></summary>

**What:** Deletes a model from local storage.<br />
**Why:** Free disk space or remove unwanted models.<br />
**How:** Replace `<model>` with the model name.<br />

**Example:**

```shell
ollama delete llama2
```

</details>

<details>
<summary><code>ollama update</code></summary>

**What:** Updates the Ollama CLI tool.<br />
**Why:** Get the latest features and bug fixes.<br />
**How:** Run this command to upgrade Ollama.<br />

**Example:**

```shell
ollama update
```

</details>

