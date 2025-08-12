
---

## Ollama Troubleshooting & Best Practices

<details>
<summary><code>Common Error: "Could not parse expression with acorn"</code></summary>

**What:** MDX parser error when rendering markdown with unescaped braces.<br />
**Why:** Curly braces like `{{ }}` in code blocks confuse the parser.<br />
**How:** Escape braces as `&#123;&#123;` and `&#125;&#125;` or wrap code in fenced blocks.<br />

**Example:**

```shell
TEMPLATE """
User: &#123;&#123; .Prompt &#125;&#125;
Assistant:
"""
```

</details>

<details>
<summary><code>Best Practice: Use Collapsible Sections</code></summary>

**What:** Organize content into expandable blocks.<br />
**Why:** Keeps documentation compact and readable.<br />
**How:** Use `<details>` and `<summary>` tags in markdown.<br />

**Example:**

```markdown
<details>
<summary>Command info</summary>
Details here...
</details>
```

</details>

<details>
<summary><code>Handling Large Models</code></summary>

**What:** Large models require significant resources.<br />
**Why:** To avoid crashes or slow performance.<br />
**How:** Use parameters like `num_ctx` to limit context size, stop unused models, and monitor system usage.<br />

**Example:**

```shell
PARAMETER num_ctx 2048
ollama stop llama2
```

</details>

<details>
<summary><code>Updating Ollama CLI</code></summary>

**What:** Keep your Ollama CLI updated.<br />
**Why:** Access newest features and security patches.<br />
**How:** Run `ollama update` regularly.<br />

**Example:**

```shell
ollama update
```

</details>

<details>
<summary><code>Backup Your Models & Configurations</code></summary>

**What:** Save your Modelfiles and custom models.<br />
**Why:** Prevent loss due to system issues.<br />
**How:** Store files in version control like GitHub.<br />

**Example:**

```bash
git init
git add Modelfile
git commit -m "Add custom model config"
```

</details>

