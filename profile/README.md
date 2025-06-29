# Horcrux

🧠 **Horcrux** is an open-source, modular, and cloud-native AI system designed to orchestrate intelligent agents using voice, plugins, LLMs, and customizable workflows.

Horcrux isn't just a framework — it’s a distributed **intelligence orchestration engine**, where every plugin, memory module, or tool is a **shard of cognition**, collectively powering flexible and persona-driven AI systems.

---

## 🔧 What Is Horcrux?

**Horcrux** enables developers to build **AI-powered assistants and agents** using:
- Pluggable skills
- Memory and context layers
- Persona-driven prompt routing
- Event-driven microservice orchestration
- Multi-modal interfaces (voice, CLI, web)

It provides the infrastructure and building blocks needed to run **intelligent, personalized, real-time AI agents** — either locally, on the edge, or in the cloud.

You can use Horcrux to build:
- Voice-first AI companions
- LLM-enhanced chatbots and agents
- Custom AI workflows using plugins + memory
- Modular AI microservices connected by queue

---

## 🧩 Key Features

- 🔌 **Plugin Engine** – Build and install skills and tools easily (`plugin.yaml`)
- 🧠 **LLM Abstraction** – Seamless use of OpenAI, Ollama, Langchain, LlamaIndex
- 🗣️ **Voice Layer** – STT (Whisper) + TTS (ElevenLabs, Coqui, Alexa)
- 🧬 **Persona System** – Persona-based prompt injection and behavior modeling
- ⚡ **Event-Driven Core** – Kafka, NATS, or Redis Streams-based async architecture
- ☸️ **Kubernetes-Native** – Microservice deployable with Helm or Kustomize
- 🔧 **CLI Tooling** – Scaffold and test plugins with `horcrux-cli`
- 🧪 **Plugin Isolation** – Run plugins via subprocess, gRPC, or Docker
- 📦 **Extensible by Design** – Custom plugins, LLM tools, adapters, and workflows

---

## 🏗️ Use Cases

- Build voice-first AI agents using open-source tools
- Create intelligent, multi-plugin LLM workflows
- Run assistants on edge devices (Raspberry Pi, Jetson, K3s)
- Use personas and memory to customize LLM interaction
- Extend with third-party APIs, smart devices, databases

---

## 📂 Architecture
<!-- 
See [`docs/architecture.md`](./docs/architecture.md) or [`diagrams/architecture.png`](./diagrams/architecture.png)

![Architecture Diagram](./diagrams/architecture.png) -->

Horcrux follows a microservices-oriented model, with individual services for LLM processing, plugin execution, memory, persona handling, and voice interaction — all orchestrated via an event queue.

---
<!-- 
## 📖 Documentation

| Page | Description |
|------|-------------|
| [System Design](docs/system-design.md) | How Horcrux works internally |
| [Architecture](docs/architecture.md) | Infra, services, deployment options |
| [Plugin Spec](docs/plugin-spec.md) | How to build and register a plugin |
| [Personas](docs/personas.md) | Customizing behavior and tone |
| [Roadmap](docs/roadmap.md) | Upcoming milestones and direction |
| [CLI Usage](docs/cli.md) | Managing the system with `horcrux-cli` |

--- -->

## 💡 How It Works

1. Voice or text input enters via adapters (CLI, Alexa, Web)
2. Input is routed to `horcrux-core` for intent handling
3. Events are published to the message queue
4. Plugin runner executes the appropriate skill/tool
5. LLMs are called when required
6. Output is returned via TTS, Web, or CLI

---

## 🧑‍💻 Contributing

Horcrux is open to contributions in:
- Plugin development
- LLM adapters and workflows
- Core engine and dispatcher enhancements
- Dev tooling, CLI, deployment automation

To get started:
- Fork this repo
- Clone and run with Docker Compose or `horcrux-cli`
- Read [`CONTRIBUTING.md`](./CONTRIBUTING.md)
- Browse open issues and discussions

---

<!-- ## 📦 Repositories in the Ecosystem

| Repo | Description |
|------|-------------|
| [`horcrux`](https://github.com/horcrux-framework/horcrux) | Core engine, orchestrator, dispatcher |
| [`horcrux-cli`](https://github.com/horcrux-framework/horcrux-cli) | Command-line tooling for dev & deploy |
| [`horcrux-plugins`](https://github.com/horcrux-framework/horcrux-plugins) | Official plugin collection (weather, jokes, system) |
| [`horcrux-llm`](https://github.com/horcrux-framework/horcrux-llm) | LLM engine & prompt formatter |
| [`horcrux-voice`](https://github.com/horcrux-framework/horcrux-voice) | Whisper + TTS integration |
| [`horcrux-deploy`](https://github.com/horcrux-framework/horcrux-deploy) | Docker + Kubernetes deployment |
| [`horcrux-docs`](https://github.com/horcrux-framework/horcrux-docs) | Documentation site and guidebooks |

--- -->

## 📜 License

Horcrux is open-source under the [Apache 2.0 License](./LICENSE).

<!-- ---

## 🌍 Join the Community

- 💬 [Discussions](https://github.com/horcrux-framework/horcrux/discussions)
- 🗺️ [Roadmap](docs/roadmap.md)
- 🧪 [Contribute a Plugin](docs/plugin-spec.md) -->
