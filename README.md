## Predict

Before implementing the routes, my predictions were:

* After sending one chat request with a **10-word user message** and asking for **32 tokens back**, I expected `usage.prompt_tokens` to be about **30 tokens** and `usage.completion_tokens` to be about **32 tokens**.

  The prompt token count is higher than the number of words because the tokenizer also adds tokens required by the model's chat template, including role and formatting tokens.

* Which of the three routes will pass its test first, with the least code?
  **`GET /health`**


* Will an unmodified `openai` Python client work against the server with only a `base_url` change?

   **Yes** ,  the server follows the OpenAI-compatible API contract, so the standard OpenAI Python client can communicate with it by changing the `base_url` to the local service. The request and response structures remain compatible with what the client expects.
