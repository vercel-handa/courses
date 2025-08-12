
---

## Ollama Run Command Options

<details>
<summary><code>ollama run &lt;model&gt; [options]</code></summary>

**What:** Run a model with various configurable options.<br />
**Why:** Customize model behavior like temperature, max tokens, stop sequences.<br />
**How:** Add flags after the model name to control execution.<br />

**Example:**

```shell
ollama run llama2 --temperature 0.5 --max_tokens 100
```

</details>

<details>
<summary><code>--temperature &lt;value&gt;</code></summary>

**What:** Sets randomness of model output.<br />
**Why:** Lower values make output deterministic; higher increase creativity.<br />
**How:** Use with `ollama run` command.<br />

**Example:**

```shell
ollama run llama2 --temperature 0.7
```

</details>

<details>
<summary><code>--max_tokens &lt;number&gt;</code></summary>

**What:** Limits maximum tokens generated.<br />
**Why:** Controls length of model output.<br />
**How:** Specify max tokens to prevent overly long answers.<br />

**Example:**

```shell
ollama run llama2 --max_tokens 150
```

</details>

<details>
<summary><code>--stop &lt;string&gt;</code></summary>

**What:** Defines stop sequence to end output.<br />
**Why:** Useful to control output boundaries.<br />
**How:** Provide a string at which model should stop.<br />

**Example:**

```shell
ollama run llama2 --stop "###"
```

</details>

<details>
<summary><code>--system &lt;string&gt;</code></summary>

**What:** Overrides system prompt temporarily.<br />
**Why:** Customize model behavior for a single run.<br />
**How:** Pass a string describing assistant role.<br />

**Example:**

```shell
ollama run llama2 --system "You are an expert assistant."
```

</details>

<details>
<summary><code>--model &lt;model&gt;</code></summary>

**What:** Explicitly specify model to run.<br />
**Why:** Useful when running from a default alias.<br />
**How:** Use to override default.<br />

**Example:**

```shell
ollama run --model llama2
```

</details>

