
---

## Ollama API Usage & Integration

<details>
<summary><code>POST /v1/chat/completions</code></summary>

**What:** Main API endpoint to get chat completions.<br />
**Why:** Allows programmatic interaction with Ollama models.<br />
**How:** Send POST request with model, messages, and parameters.<br />

**Example:**

```json
POST /v1/chat/completions
{
  "model": "llama2",
  "messages": [{"role": "user", "content": "Hello Ollama!"}],
  "temperature": 0.7,
  "max_tokens": 150
}
```

</details>

<details>
<summary><code>Authorization Header</code></summary>

**What:** API key authentication.<br />
**Why:** Secure access control.<br />
**How:** Send `Authorization: Bearer &lt;API_KEY&gt;` header.<br />

**Example:**

```http
Authorization: Bearer your_api_key_here
```

</details>

<details>
<summary><code>Messages Format</code></summary>

**What:** Structure conversation history.<br />
**Why:** Maintain context and roles.<br />
**How:** Array of message objects with `role` and `content`.<br />

**Example:**

```json
[
  {"role": "system", "content": "You are a helpful assistant."},
  {"role": "user", "content": "Tell me a joke."}
]
```

</details>

<details>
<summary><code>Optional Parameters</code></summary>

**What:** Customize API responses.<br />
**Why:** Control output style and length.<br />
**How:** Include keys like `temperature`, `max_tokens`, `stop`.<br />

**Example:**

```json
{
  "temperature": 0.6,
  "max_tokens": 100,
  "stop": ["\n"]
}
```

</details>

<details>
<summary><code>Example cURL Request</code></summary>

**What:** How to call API from terminal.<br />
**Why:** Quick test and automation.<br />
**How:** Use `curl` with headers and JSON body.<br />

**Example:**

```bash
curl -X POST https://api.ollama.com/v1/chat/completions \
-H "Authorization: Bearer your_api_key_here" \
-H "Content-Type: application/json" \
-d '{
  "model": "llama2",
  "messages": [{"role": "user", "content": "Hello Ollama!"}],
  "temperature": 0.7,
  "max_tokens": 150
}'
```

</details>

