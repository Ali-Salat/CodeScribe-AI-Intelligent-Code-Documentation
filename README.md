# 📝 CodeScribe AI – Intelligent Code Documentation

An AI-powered multi-agent system built entirely with **JacLang** and **ByLLM** that automatically generates comprehensive, human-readable documentation for any GitHub repository.

## What It Does

CodeScribe AI clones a GitHub repo, analyzes its structure and dependencies, builds a Code Context Graph, and produces clean Markdown documentation with visual diagrams—all automatically using Jac's native agentic framework.

## Architecture

Powered by **JacLang's** agentic programming model and **ByLLM** for AI capabilities, the system coordinates four specialized agents:

- **🧠 Supervisor** – Orchestrates the entire documentation workflow
- **🗂 Repo Mapper** – Clones repositories and maps directory structures  
- **🔍 Code Analyzer** – Parses source code and builds dependency graphs
- **✍️ DocGenie** – Generates structured Markdown docs and diagrams

## Quick Start

```bash
# Clone and setup
git clone <repo_url>
cd codescribe-ai

# Install JacLang
pip install jaclang

# Configure
cp .env.example .env
# Edit .env with your ByLLM API configuration

# Launch
jac serve main.jac
```

## Usage

Generate documentation for any GitHub repository:

```bash
curl -X POST http://localhost:8000/api/supervisor/run \
  -H "Content-Type: application/json" \
  -d '{"repo_url":"https://github.com/psf/requests"}'
```

Documentation output: `outputs/requests/docs.md`

## Key Features

✓ **Pure JacLang implementation** – Leverages Jac's native agentic programming  
✓ **ByLLM integration** – Seamless AI model orchestration  
✓ **Multi-agent coordination** – Walker-based agent communication  
✓ **Code Context Graphs** – Intelligent dependency mapping  
✓ **Automatic diagram generation** – Visual code relationships  
✓ **Graph-based architecture** – Natural fit for Jac's data spatial paradigm

## Why JacLang + ByLLM?

**JacLang** provides a revolutionary agentic programming model perfect for multi-agent systems, while **ByLLM** offers flexible LLM integration without external dependencies. Together, they enable:

- Native agent-to-agent communication via walkers
- Graph-based code representation (nodes + edges)
- Seamless LLM orchestration through ByLLM
- Clean, declarative agent definitions

## Roadmap

- **Multi-language support** – JavaScript, Go, TypeScript, Rust
- **Enhanced analysis** – Complexity metrics and code quality indicators
- **Interactive documentation** – Live code examples and API references
- **ByLLM model flexibility** – Support for multiple LLM providers

## Tech Stack

**JacLang** – Agentic programming language  
**ByLLM** – LLM integration framework  
**Tree-sitter** – Code parsing  
**Graphviz** – Diagram generation

---

**License:**  
**Version:** 1.0.0  
*Agentic documentation powered by JacLang and ByLLM*
