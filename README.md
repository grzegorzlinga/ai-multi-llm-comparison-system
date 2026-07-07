# AI Multi-LLM Comparison System

An automated AI benchmarking workflow built with Make.com and n8n.

This project sends a single prompt to both OpenAI GPT and Google Gemini, evaluates both responses using an AI Judge, stores benchmark results in Google Sheets, and returns structured JSON to the client.

---

# Architecture

![Architecture](ai-multi-llm-architecture.png)

---

# Workflow

1. Receive request through Make Webhook
2. Forward request to n8n
3. Send prompt to OpenAI
4. Send prompt to Google Gemini
5. AI Judge compares both responses
6. Select the better answer
7. Return JSON to Make
8. Save benchmark results to Google Sheets

---

# Screenshots

## Make Scenario

![Make Workflow](01_make_workflow.png)

---

## n8n Workflow

![n8n Workflow](02_n8n_workflow.png)

---

## API Response (ReqBin)

![ReqBin](reqbin-response.png)

---

## Benchmark Results

![Benchmark Results](06-benchmark-results.png)

---

# Technologies

- Make.com
- n8n
- OpenAI API
- Google Gemini API
- Google Sheets
- HTTP Webhooks
- JSON

---

# Features

- Multi-LLM comparison
- AI Judge evaluation
- Automatic winner selection
- Benchmark storage
- REST API endpoint
- End-to-end automation
