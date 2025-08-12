
---

## Ollama Modelfile Syntax & Parameters

<details>
<summary><code>ollama create mymodel -f Modelfile</code></summary>

**What:** Create a custom model from a Modelfile.<br />
**Why:** Lets you modify parameters, system prompts, and templates.<br />
**How:** Write a `Modelfile` with your settings, then run this command.<br />

**Example:**

```shell
FROM llama2:7b
PARAMETER temperature 0.7
SYSTEM "You are a helpful assistant."
```

</details>

<details>
<summary><code>ollama run mymodel</code></summary>

**What:** Runs your custom model.<br />
**Why:** Test and interact with your modified model.<br />
**How:** Use after creating the model.<br />

**Example:**

```shell
ollama run mymodel
```

</details>

<details>
<summary><code>FROM llama2:7b</code></summary>

**What:** Defines base model in Modelfile.<br />
**Why:** All custom models must start from a base.<br />
**How:** First line of your `Modelfile`.<br />

**Example:**

```shell
FROM llama2:7b
```

</details>

<details>
<summary><code>PARAMETER temperature 0.7</code></summary>

**What:** Controls randomness of output.<br />
**Why:** Adjusts creativity (0.0 = deterministic, 1.0 = very creative).<br />
**How:** Add inside `Modelfile`.<br />

**Example:**

```shell
PARAMETER temperature 0.7
```

</details>

<details>
<summary><code>PARAMETER num_ctx 2048</code></summary>

**What:** Sets maximum context tokens.<br />
**Why:** Allows longer memory in conversations.<br />
**How:** Inside `Modelfile`.<br />

**Example:**

```shell
PARAMETER num_ctx 2048
```

</details>

<details>
<summary><code>PARAMETER stop "###"</code></summary>

**What:** Defines stop sequence.<br />
**Why:** Stops output when marker is reached.<br />
**How:** Inside `Modelfile`.<br />

**Example:**

```shell
PARAMETER stop "###"
```

</details>

<details>
<summary><code>SYSTEM "You are a helpful assistant."</code></summary>

**What:** Defines system prompt.<br />
**Why:** Keeps tone/personality consistent.<br />
**How:** Inside `Modelfile`.<br />

**Example:**

```shell
SYSTEM "You are a helpful assistant."
```

</details>

<details>
<summary><code>TEMPLATE """  
User: &#123;&#123; .Prompt &#125;&#125;  
Assistant:  
"""</code></summary>

**What:** Sets prompt structure.<br />
**Why:** Enforces consistent I/O formatting.<br />
**How:** Inside `Modelfile`.<br />

**Example:**

```shell
TEMPLATE """
User: {{ .Prompt }}
Assistant:
"""
```

</details>

<details>
<summary><code>LICENSE "MIT"</code></summary>

**What:** Adds license information.<br />
**Why:** Clarifies usage rights.<br />
**How:** Inside `Modelfile`.<br />

**Example:**

```shell
LICENSE "MIT"
```

</details>

<details>
<summary><code>MESSAGE "Trained on 2023 company FAQ."</code></summary>

**What:** Adds a permanent note in the model history.<br />
**Why:** Stores metadata about training/data origin.<br />
**How:** Inside `Modelfile`.<br />

**Example:**

```shell
MESSAGE "Trained on 2023 company FAQ."
```

</details>

---

