[EN] English | [FA](./README.md)

# Rahyana Examples Hub ✨

Welcome to the official hub for Rahyana example repositories. This repo links to language-specific examples so you can start fast and pick the best path for your stack.

## 📎 Common API notes
- **Base URL**: `https://rahyana.ir/api/v1`
- **Auth**: header `Authorization: Bearer YOUR_API_KEY`
- **Models**: list with `GET /api/v1/models`
- **Errors**: response contains `error.message`, `error.type`, `error.code`; provider detail may appear in header `X-Provider-Error`.
- **Local testing**: set `API_KEY_OVERRIDE` and `BASE_URL_OVERRIDE`

### 🧪 Sample request (cURL) — list models

```bash
curl -s -H "Authorization: Bearer $API_KEY" \
     "https://rahyana.ir/api/v1/models"
```

### 🧪 Sample request (cURL) — chat completions
```bash
curl -s -X POST "https://rahyana.ir/api/v1/chat/completions" \
     -H "Authorization: Bearer $API_KEY" \
     -H "Content-Type: application/json" \
     -d '{
       "model": "openai/gpt-4o",
       "messages": [{"role":"user","content":"hello"}]
     }'
```

## 🤝 OpenAI compatibility
- Paths and request/response structures align with OpenAI’s API, so many OpenAI clients can work by switching the base URL and key.
- For special modes (image/audio/PDF, tool calling), Rahyana provides compatibility mappings.

## 🧠 More docs
- Models: `docs/models.en.md` (Farsi version: `docs/models.fa.md`)
- Chat completions: `docs/chat-completions.en.md` (Farsi version: `docs/chat-completions.fa.md`)

## 📚 Language repos
- JavaScript: coming soon
- TypeScript: coming soon
- Python: coming soon

## 🧩 What’s inside
- Chat completions (Basic/Streaming/JSON Mode) and image/audio/PDF inputs
- Real-world projects (content generator, chatbot, code assistant, ...)
- Dev tools (test generator, performance monitor, docs generator, code review, CI/CD)

## ✅ Quality standards
- Examples are runnable and documented (FA/EN)
- Smoke tests for reliability
- Standard formatting and linting (Black/Ruff, ESLint/Prettier)

## 🤝 Contributing
- Report bugs or improvements via Issues
- Share ideas in Discussions
- Contribution guide: `CONTRIBUTING.md`

---

<!-- SEO keywords: Rahyana AI examples, GPT-5, GPT-4o, OpenAI-compatible, JSON Mode, streaming, AI chatbot, content generator, Python, TypeScript, JavaScript -->
