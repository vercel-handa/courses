
---

## Ollama CLI Essentials


<details>
<summary><code>ollama --version</code></summary>

**What:** Shows the installed Ollama CLI version.<br />
**Why:** Verify your Ollama version to ensure compatibility.<br />
**How:** Run in your terminal.<br />

**Example:**

```shell
ollama --version
```

</details>

<details>
<summary><code>ollama pull &lt;model&gt;</code></summary>

**What:** Downloads a model from the Ollama registry.<br />
**Why:** You need the model locally to run it.<br />
**How:** Replace `<model>` with the model name.<br />

**Example:**

```shell
ollama pull llama2
```

</details>

<details>
<summary><code>ollama run &lt;model&gt;</code></summary>

**What:** Runs the specified model locally.<br />
**Why:** Interact with the model to generate text.<br />
**How:** Replace `<model>` with the model name.<br />

**Example:**

```shell
ollama run llama2
```

</details>

<details>
<summary><code>ollama list</code></summary>

**What:** Lists all locally installed models.<br />
**Why:** Check which models you have.<br />
**How:** Run in terminal.<br />

**Example:**

```shell
ollama list
```

</details>

<details>
<summary><code>ollama stop &lt;model&gt;</code></summary>

**What:** Stops a running model.<br />
**Why:** Free system resources.<br />
**How:** Replace `<model>` with the model name.<br />

**Example:**

```shell
ollama stop llama2
```

</details>

<details>
<summary><code>ollama delete &lt;model&gt;</code></summary>

**What:** Deletes a model from local storage.<br />
**Why:** Free up disk space.<br />
**How:** Replace `<model>` with the model name.<br />

**Example:**

```shell
ollama delete llama2
```

</details>

![Ollama Essentials](/img/ollama/011-ollama.png)

