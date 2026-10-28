# Krishna Shukla

Backend and infrastructure engineer working in TypeScript and Go, with a focus on dependable AI and real-time systems.

I am a student developer in India, graduating in May 2027. I like problems involving failure handling, event pipelines, and systems that need to stay useful under imperfect conditions, and I am looking for backend, infrastructure, and voice AI roles.

## Highlights

- Paid Internet Archive Fellow contributing to [OpenLibrary](https://github.com/internetarchive/openlibrary).
- [34 merged pull requests](https://github.com/pulls?q=is%3Apr+author%3AKrishnaShuk+is%3Amerged) across 14 repositories, verified from GitHub.
- Designed and merged LiveKit's [LLM FallbackAdapter](https://github.com/livekit/agents-js/pull/916), which tries providers in priority order, marks failures unavailable, and probes recovery with a real request.
- Shipped 10 merged PRs to [LiveKit agents-js](https://github.com/livekit/agents-js), covering LLM failover, Deepgram Flux support, worker sizing, and audio-stream cleanup.

## Selected work

### [VoxObs](https://github.com/KrishnaShuk/VoxObs)

A TypeScript toolkit for observing LiveKit voice agents, attributing latency and failures across STT, LLM, TTS, endpointing, and voice-to-voice turns.

It carries 16 typed event kinds over WebSockets, buffers up to 10,000 events for reconnect and replay, and stores idempotently in Postgres by session sequence. The repository includes a LiveKit agent, Express ingest service, live Next.js timeline, session replay, OpenTelemetry instrumentation, failure injection, and CI.

*Stack: TypeScript, LiveKit agents-js, Express, WebSockets, Postgres, Next.js, OpenTelemetry.*

### [EVM TX Safety](https://github.com/KrishnaShuk/evm-tx-safety)

An MIT-licensed pre-signing transaction analyzer for EVM chains, available as a web app, HTTP API, and `evm-safety check` CLI.

It decodes calldata and recursively inspects multicalls, then simulates through Tenderly, `debug_traceCall`, or `eth_call` and scores findings with explainable rules. It supports Ethereum, Base, Arbitrum, Optimism, Polygon, and BNB Chain.

*Stack: TypeScript, ethers v6, Next.js, JSON-RPC, Tenderly, GitHub Actions.*

### [PdfPod](https://github.com/KrishnaShuk/Pdfpod-client)

A document assistant that answers questions over uploaded PDFs and turns them into audio summaries.

Long-running work is separated from the API through BullMQ and Redis: a worker uses Gemini, Qdrant, Google Cloud Text-to-Speech, and Cloudflare R2 while the client polls job status.

*Stack: TypeScript, Next.js, Express, BullMQ, Redis, MongoDB, Qdrant.*

## Open source

- **[LiveKit agents-js](https://github.com/livekit/agents-js)**: [FallbackAdapter](https://github.com/livekit/agents-js/pull/916), [Deepgram Flux STT v2](https://github.com/livekit/agents-js/pull/938), and an [AudioResampler lifecycle fix](https://github.com/livekit/agents-js/pull/1453).
- **[OpenLibrary](https://github.com/internetarchive/openlibrary)**: six merged PRs, including [evicting failed search carousels from cache](https://github.com/internetarchive/openlibrary/pull/11900) and [language-aware random books](https://github.com/internetarchive/openlibrary/pull/11630).
- **[PEcAn](https://github.com/PecanProject/pecan)**: two merged PRs that replaced manually managed test directories with automatically cleaned temporary directories.
- **[cx-core](https://github.com/cxlinux-ai/cx-core)**: added [retry classification with exponential backoff](https://github.com/cxlinux-ai/cx-core/pull/658) and an [interactive troubleshooting assistant](https://github.com/cxlinux-ai/cx-core/pull/584).

See all [merged pull requests](https://github.com/pulls?q=is%3Apr+author%3AKrishnaShuk+is%3Amerged).

## Stack

**Languages:** TypeScript, Go. **Backend and data:** Node.js, Express, WebSockets, Postgres, MongoDB, Redis, Qdrant.

**Infra and tooling:** Docker, GitHub Actions, OpenTelemetry, pnpm workspaces, Git.

## Contact

[shuklakrishna.kris@gmail.com](mailto:shuklakrishna.kris@gmail.com) · [LinkedIn](https://in.linkedin.com/in/krishna-shuk)

Open to backend, infrastructure, and voice AI roles after May 2027, and internships earlier.
