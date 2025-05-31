# Cordia API
Cordia models are general purpose AI models, designed specifically for AI characters and daily conversations.

## What is Cordia API?
Cordia API provides a programmatic way to integrate Cordia models into your application as a developer. It follows the OpenAI-compatible API standard, making it easy to implement with existing libraries and SDKs.

## Demos
There are some projects by the developer community that use Cordia API to create authentic Human to AI conversations

## Getting Started
You will need to generate an API Key on the Dashboard (SOON).

## Implementation Examples
### 🐍 Python
```python
from openai import OpenAI
client = OpenAI(
  base_url="https://api.aicordapp.com/api/v1",
  api_key="<YOUR-API-KEY>",
)
completion = client.chat.completions.create(
  model="cordia-a6",
  messages=[
      {
        "role": "system",
        "content": "You are a helpful AI character."
      },
    {
      "role": "user",
      "content": "What is the meaning of life?"
    }
  ]
)
print(completion)
print(completion.choices[0].message.content)
```

