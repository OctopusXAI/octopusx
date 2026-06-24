# octopusx
One OpenAI-compatible API for 200+ AI models — GPT, Claude, Gemini &amp; more

markdown
# OctopusX 🐙
One OpenAI-compatible API for 200+ AI models — GPT, Claude, Gemini & more

Access GPT-5, Gemini 3, MiniMax, Claude and hundreds of LLMs through a single endpoint. Fully compatible with official OpenAI SDK, switch models by only changing one parameter, no vendor lock-in.

## ⚡ Quick Start & Installation
### 1. Install dependency
```bash
# Python
pip install openai

# Node.js
npm install openai
2. Python Usage Example
python
运行
from openai import OpenAI

client = OpenAI(
    api_key="YOUR_OCTOPUSX_KEY",
    base_url="https://octopusx.ai"
)

response = client.chat.completions.create(
    model="gpt-5",
    messages=[{"role": "user", "content": "Introduce OctopusX briefly"}]
)
print(response.choices[0].message.content)
3. Node.js Usage Example
javascript
运行
import OpenAI from "openai";

const client = new OpenAI({
  apiKey: process.env.OCTOPUSX_KEY,
  baseURL: "https://octopusx.ai"
});

async function runChat() {
  const result = await client.chat.completions.create({
    model: "gemini-3-flash",
    messages: [{ role: "user", content: "Test multi-model API" }]
  });
  console.log(result.choices[0].message.content);
}
runChat();
📌 Core Features
Single unified API endpoint for all mainstream LLMs
Drop-in OpenAI SDK compatibility, zero migration cost
Consolidated unified billing for all model consumption
Simple model switching without rewriting request logic
Built-in token usage statistics & cost dashboard
🎯 Suitable Scenarios
Backend AI production service
Multi-model performance comparison & testing
AI chatbot, content generation tools development
Enterprise unified LLM access gateway
🔗 Official Links
Website: https://octopusx.ai
Documentation: https://doc.octopusx.ai/en
Contact: hello@octopusx.ai
