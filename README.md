## Predict

Before implementing the routes, my predictions were:

* After sending one chat request with a **10-word user message** and asking for **32 tokens back**, I expected `usage.prompt_tokens` to be about **30 tokens** and `usage.completion_tokens` to be about **32 tokens**.

* Which of the three routes will pass its test first, with the least code?
  **`GET /health`**

* Will an unmodified `openai` Python client work against the server with only a `base_url` change?

   **Yes** ,  the server follows the OpenAI-compatible API contract, so the standard OpenAI Python client can communicate with it by changing the `base_url` to the local service. The request and response structures remain compatible with what the client expects.

  Step 1:
  
  <img width="648" height="150" alt="image" src="https://github.com/user-attachments/assets/e8f77601-6697-4fd4-be00-72520cf03982" />

  Step 2:

  <img width="770" height="129" alt="image" src="https://github.com/user-attachments/assets/d7560bc8-8716-4d34-bc53-d50bb3a0f5cf" />

  Step 3:

  <img width="766" height="181" alt="WhatsApp Image 2026-08-24 at 4 33 33 PM" src="https://github.com/user-attachments/assets/f2602237-f8da-4d87-acbe-93be36fd34ec" />

  Step 4:

  <img width="441" height="65" alt="{EC6D5548-C777-4817-BA09-4785759DB510}" src="https://github.com/user-attachments/assets/285fafb9-7189-498a-a381-d672bcc4803f" />


  Step 5:

  <img width="883" height="213" alt="WhatsApp Image 2026-08-24 at 4 44 01 PM" src="https://github.com/user-attachments/assets/e6e43a2c-6e24-40b8-ab85-4f8e96af8cb5" />


  
