# HandsOnAPIs-Python-FastAPI-Examples-Book

![Project Banner Placeholder](https://via.placeholder.com/1200x300/0D1117/FFFFFF?text=Hands-On+APIs+for+AI+and+Data+Science+Source+Code)

<p align="center">
    <a href="https://github.com/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book/stargazers">
        <img src="https://img.shields.io/github/stars/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book?style=flat-square&logo=github" alt="GitHub Stars">
    </a>
    <a href="https://github.com/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book/actions/workflows/ci.yml">
        <img src="https://img.shields.io/github/actions/workflow/status/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book/ci.yml?label=Build&style=flat-square" alt="Build Status">
    </a>
    <a href="https://codecov.io/gh/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book">
        <img src="https://img.shields.io/codecov/c/gh/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book?style=flat-square" alt="Code Coverage">
    </a>
    <img src="https://img.shields.io/badge/Language-Python%203.10%2B-blue?style=flat-square" alt="Python Version">
    <img src="https://img.shields.io/badge/Framework-FastAPI%20v0.118.0%2B-green?style=flat-square" alt="FastAPI Version">
    <a href="https://github.com/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book/blob/main/LICENSE">
        <img src="https://img.shields.io/badge/License-CC%20BY--NC%204.0-orange?style=flat-square" alt="License">
    </a>
</p>

--- 

This repository contains the complete, production-grade source code examples accompanying the **'Hands-On APIs for AI and Data Science'** educational material, specifically covering Part 1: Robust Python and FastAPI API construction.

It is engineered to demonstrate best practices in modern API design, performance tuning, dependency management using `uv`, and secure integration patterns required for Data Science and Machine Learning endpoints.

[⭐ Star ⭐ this Repo if you find the patterns valuable for your professional work.]

## 📋 Table of Contents

1.  [Introduction & Vision](#introduction--vision)
2.  [Architectural Blueprint](#architectural-blueprint)
3.  [Apex Technical Directives](#apex-technical-directives)
4.  [Technology Stack](#technology-stack)
5.  [Development & Setup](#development--setup)
6.  [Verification & Testing](#verification--testing)
7.  [License](#license)

---

## Introduction & Vision

The core vision of this codebase is to transition developers from basic API scaffolding to building **enterprise-ready, high-performance, and AI-aware microservices** using Python and FastAPI. Every file exemplifies a mature design choice.

## Architectural Blueprint

The repository structure adheres to a **Modular Monolith** pattern, suitable for rapid iteration while maintaining clear boundaries for scaling components (e.g., separating data loading, core processing, and external API interactions).

ascii
/hands_on_apis/
├── core/              # Core application setup (settings, logging, lifecycle)
│   ├── config.py
│   └── database.py
├── modules/           # Business logic modules (Modular Monolith boundary)
│   ├── ai_processing/ # Integration layer for ML/AI models
│   │   └── endpoints.py
│   └── data_ingestion/
│       └── endpoints.py
├── api/               # FastAPI Routers and main application entry
│   └── router.py
├── tests/             # Comprehensive Pytest suites
│   └── test_endpoints.py
├── .gitignore
├── pyproject.toml     # uv/Ruff/Poetry configuration
└── README.md


## Apex Technical Directives

<details>
<summary><strong>🤖 AI Agent Directives (December 2025 Standard)</strong></summary>

# SYSTEM: APEX TECHNICAL AUTHORITY & ELITE ARCHITECT (DECEMBER 2025 EDITION)

## 1. IDENTITY & PRIME DIRECTIVE
**Role:** You are a Senior Principal Software Architect and Master Technical Copywriter with **40+ years of elite industry experience**. You operate with absolute precision, enforcing FAANG-level standards and the wisdom of "Managing the Unmanageable."
**Context:** Current Date is **December 2025**. You are building for the 2026 standard.
**Output Standard:** Deliver **EXECUTION-ONLY** results. No plans, no "reporting"—only executed code, updated docs, and applied fixes.
**Philosophy:** "Zero-Defect, High-Velocity, Future-Proof."

---

## 2. INPUT PROCESSING & COGNITION
*   **SPEECH-TO-TEXT INTERPRETATION PROTOCOL:**
    *   **Context:** User inputs may contain phonetic errors (homophones, typos).
    *   **Semantic Correction:** **STRICTLY FORBIDDEN** from executing literal typos. You must **INFER** technical intent based on the project context.
    *   **Logic Anchor:** Treat the `README.md` as the **Single Source of Truth (SSOT)**.
*   **MANDATORY MCP INSTRUMENTATION:**
    *   **No Guessing:** Do not hallucinate APIs. Do not invent library versions.
    *   **Research First:** Use `linkup`/`brave` to search for **December 2025 Industry Standards**, **Security Threats**, and **2026 Architectural Trends** related to FastAPI and AI endpoints.
    *   **Validation:** Use `docfork` to verify *every* external API signature (e.g., Google Gemini, Database drivers).
    *   **Reasoning:** Engage `clear-thought-two` to architect complex asynchronous flows *before* writing code.

---

## 3. CONTEXT-AWARE APEX TECH STACKS (LATE 2025 STANDARDS)
**Directives:** Detect the project type (`pyproject.toml` for Python) and apply the corresponding **Apex Toolchain**.

*   **PRIMARY SCENARIO: DATA / SCRIPTS / AI (Python)**
    *   **Stack:** This project leverages **Python 3.11+ (Minimum)**. Key tools include **uv** (for package management and dependency resolution, preferred over Poetry/Pipenv), **Ruff** (for ultra-fast linting, formatting, and static analysis), and **Pytest** (for robust unit and integration testing). Use `pydantic_settings` for configuration loading.
    *   **Architecture:** Adheres to a **Modular Monolith** pattern, ensuring clear separation of concerns (SOLID principles applied rigorously). All external services must be implemented via Ports and Adapters (Hexagonal principles) where applicable, abstracting database/AI connections.
    *   **AI Integration:** Assume deep integration with **OpenAI/Gemini APIs**. All API calls must be asynchronous (`httpx`, `asyncio`) and include exponential backoff retries for resilience.
    *   **CLI Framework:** If a CLI exists, it must utilize **Typer** for clean, type-hinted CLI definition.

## 4. DEVELOPMENT PRINCIPLES
*   **SOLID:** Absolutely mandatory. Favor Dependency Injection (DI) over global state.
*   **DRY:** Avoid boilerplate. Leverage FastAPI's built-in features (dependency injection, schemas).
*   **YAGNI:** Only build what is currently required by the book examples. Future-proofing means maintainability, not feature creep.
*   **SECURITY:** Never hardcode secrets. Use environment variables loaded via `pydantic-settings` or an equivalent secure configuration loader.

## 5. VERIFICATION & VALIDATION
*   **Linting/Formatting:** Enforce 100% compliance with **Ruff** configuration defined in `pyproject.toml`. Fix on save/pre-commit.
*   **Testing:** Achieve **>90% Unit Test Coverage** using `Pytest`. Integration tests must mock all external HTTP/AI calls.
*   **Build Verification Command:** `uv run pytest --cov`

</details>

## Technology Stack

| Component | Technology | Purpose |
| :--- | :--- | :--- |
| Core Framework | FastAPI | High-performance asynchronous web framework. |
| Language | Python 3.11+ | Modern, type-hinted standard. |
| Dependency Management | **uv** (v0.4.x+) | Fast resolution and installation. |
| Linting/Formatting | **Ruff** | Unified, speed-optimized static analysis. |
| Testing | **Pytest** | Unit, integration, and dependency testing. |
| Data Validation | Pydantic V2 | Strict data modeling and serialization. |
| Asynchrony | `asyncio`/`httpx` | Non-blocking I/O for external services. |

## Development & Setup

Follow the Apex standard for pristine environment setup. This ensures future compatibility and reproducible builds.

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book.git
    cd HandsOnAPIs-Python-FastAPI-Examples-Book
    

2.  **Environment Setup (Using uv):
    **
    We mandate isolated virtual environments.
    bash
    # Create and activate environment
    uv venv
    source .venv/bin/activate  # Linux/macOS
    # .venv\Scripts\activate  # Windows

    # Install dependencies based on pyproject.toml
    uv sync
    

3.  **Run Locally (Example):
    **
    Assuming the core application is accessible via `main.py` or similar entry point defined in the examples.
    bash
    # Start the Uvicorn server with hot-reloading
    uvicorn api.router:app --reload --host 0.0.0.0 --port 8000
    

### Development Scripts

| Command | Description |
| :--- | :--- |
| `uv run build` | Installs dependencies and builds required artifacts. |
| `uv run format` | Applies Ruff formatting rules across the entire codebase. |
| `uv run lint` | Runs all Ruff static analysis checks (security, performance, style). |
| `uv run pytest` | Executes all unit and integration tests with coverage reporting. |

## Verification & Testing

Robustness is verified through automated pipelines.

1.  **Code Quality Check:** Run `uv run lint` to satisfy Ruff standards.
2.  **Unit/Integration Testing:** Run `uv run pytest --cov` to ensure >90% coverage on all modular components.
3.  **API Contract Validation:** Use the generated OpenAPI/Swagger UI (`/docs`) to manually verify endpoint contracts against the book's specifications.

## License

This project is licensed under the **Creative Commons Attribution-NonCommercial 4.0 International License**. See the [LICENSE](LICENSE) file for full details.
