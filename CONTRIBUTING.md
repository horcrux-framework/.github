# Contributing to Horcrux

Thank you for considering contributing to **Horcrux**! 🧠  
Horcrux is a modular, voice-first, plugin-powered AI framework — and it's made stronger with community collaboration.

---

## 📁 Repository Structure

This GitHub organization is structured into modular repositories:

| Repo               | Purpose                                           |
|--------------------|---------------------------------------------------|
| `horcrux`           | Docs and system overview                         |
| `horcrux-core`      | Core orchestrator, persona manager, plugin hub   |
| `horcrux-cli`       | Developer CLI tools                              |
| `horcrux-llm`       | Langchain/OpenAI/Ollama integration              |
| `horcrux-voice`     | STT/TTS modules (Whisper, ElevenLabs)            |
| `horcrux-plugins`   | Official and contributed plugins                 |
| `horcrux-deploy`    | Docker/Kubernetes deployment resources           |

---

## 🚀 Getting Started

1. Fork & Clone

   git clone https://github.com/your-username/horcrux-tools.git
   cd horcrux-tools

2. Create a Branch

   git checkout -b feat/your-feature-name

3. Develop Locally
- Use `docker-compose up` to start local services
<!-- - Or use `horcrux-cli` for plugin testing and system simulation -->

4. Commit Using Conventional Commits (see below)

5. Push & Open a Pull Request

---

## ✅ Commit Conventions (Required)

We follow the Conventional Commits specification for clarity, automation, and changelogs.

Use the helper aliases provided in your shell environment:

| Type      | Alias       | Description                           |
|-----------|-------------|---------------------------------------|
| Feature   | gfeat       | Adds a new feature                    |
| Fix       | gfix        | Bug fix or issue resolution           |
| Docs      | gdocs       | Documentation changes                 |
| Style     | gstyle      | Formatting, whitespace, etc.          |
| Refactor  | grefactor   | Code structure changes                |
| Perf      | gperf       | Performance improvements              |
| Test      | gtest       | Add or improve test coverage          |
| Build     | gbuild      | Build system or dependency changes    |
| CI        | gci         | Continuous Integration changes        |
| Chore     | gchore      | Non-functional changes                |
| Revert    | grevert     | Reverts a previous commit             |

Examples:

- gfeat "auth" "Add JWT token refresh support"
- gfix "" "Fix TTS crash on empty string"
- gdocs "readme" "Document plugin scaffold CLI usage"


---

<!-- ## 🧩 Plugin Contributions

Want to build your own AI skill or capability?

   horcrux plugin create my-skill

Then test it:

   horcrux plugin test ./my-skill

Each plugin should include:
- A `plugin.yaml` manifest
- A `README.md`
- Optional `config.schema.json` if it supports UI
- Tests or usage examples

Submit a PR to `horcrux-plugins` and the core team will review and onboard it!

--- -->

## 🛠 Code Guidelines

- Follow modular boundaries and plugin specs
- Write unit tests for new functionality
- Format code (e.g., `prettier`, `black`)
- Keep commits atomic and descriptive
- Use `.env.example` to document configs

---

<!-- ## 🧪 Local Development

You can run Horcrux services via Docker:

   docker-compose up

Or launch specific plugins/tools using:

   horcrux plugin run ./plugins/my-skill

Each service repo may include `README.md` with runtime or build instructions.

--- -->

## 💬 Community & Support

- Open an Issue for bugs or enhancements
- Use Discussions to ask or suggest

---

## 🙏 Code of Conduct

Please review our Code of Conduct in the .github repo.  
We’re committed to fostering a respectful and inclusive environment.

---

## 📜 License

By contributing to this project, you agree that your contributions will be licensed under the Apache 2.0 License.

---

Thanks for helping make Horcrux smarter, stronger, and more open for all. 🌍
