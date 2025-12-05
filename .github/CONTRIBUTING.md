# Contributing to HandsOnAPIs-Python-FastAPI-Examples-Book

We welcome contributions to enhance the `HandsOnAPIs-Python-FastAPI-Examples-Book` repository. This project adheres to strict architectural and quality standards, ensuring a robust and maintainable codebase. All contributions must align with these principles and the directives outlined in `AGENTS.md`.

## 1. Code of Conduct

This project has adopted the Contributor Covenant as its Code of Conduct. Please review the [CODE_OF_CONDUCT.md](https://github.com/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book/blob/main/CODE_OF_CONDUCT.md) to understand the expected standards of behavior.

## 2. Core Principles & Architecture

Our development philosophy is "Zero-Defect, High-Velocity, Future-Proof." We aim for clarity, maintainability, and adherence to best practices. Key architectural drivers include:

*   **Python 3.10+:** Leveraging modern Python features.
*   **FastAPI:** For building high-performance, asynchronous APIs.
*   **uv & Ruff:** For efficient package management and lightning-fast linting/formatting.
*   **Pytest:** For comprehensive testing.
*   **Modular Design:** Ensuring components are loosely coupled and highly cohesive.

Refer to `AGENTS.md` for a detailed breakdown of the technical stack, architectural patterns (e.g., SOLID, DRY), and verification commands.

## 3. How to Contribute

### 3.1. Reporting Bugs

If you find a bug, please open an issue on GitHub using the provided **Bug Report template** (`.github/ISSUE_TEMPLATE/bug_report.md`). Be sure to include:

*   A clear and descriptive title.
*   Detailed steps to reproduce the bug.
*   The expected behavior versus the actual behavior.
*   Relevant environment information (e.g., Python version, FastAPI version).
*   Screenshots or logs if applicable.

### 3.2. Suggesting Enhancements or Features

We welcome suggestions for new features or improvements. Please open an issue using the **Feature Request template** (`.github/ISSUE_TEMPLATE/feature_request.md`). Provide a clear explanation of the proposed change and its benefits.

### 3.3. Submitting Code Changes (Pull Requests)

We encourage you to submit code changes via Pull Requests (PRs).

1.  **Fork the Repository:** Create a fork of the `chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book` repository.
2.  **Create a New Branch:** From your fork, create a descriptive branch for your changes (e.g., `feature/add-new-api-example`, `fix/resolve-fastapi-validation-error`).
3.  **Make Your Changes:** Implement your feature or fix. Ensure your code adheres to the project's coding style and standards.
4.  **Test Your Changes:** Write and run tests using `pytest` to ensure your changes do not introduce regressions and meet requirements. All tests must pass.
5.  **Lint and Format:** Run `ruff check --fix` and `ruff format` to ensure code quality and consistency.
6.  **Commit Your Changes:** Write clear and concise commit messages.
7.  **Push to Your Fork:** Push your branch to your fork on GitHub.
8.  **Open a Pull Request:** Open a Pull Request from your fork's branch to the `main` branch of the `chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book` repository.
    *   **PR Template:** Use the provided Pull Request template (`.github/PULL_REQUEST_TEMPLATE.md`) to guide your submission.
    *   **Description:** Clearly explain the purpose of your PR, the changes made, and how to test them.

## 4. Development Environment Setup

To set up your local development environment, follow these steps:

1.  **Clone the Repository:**
    bash
    git clone https://github.com/chirag127/HandsOnAPIs-Python-FastAPI-Examples-Book.git
    cd HandsOnAPIs-Python-FastAPI-Examples-Book
    

2.  **Set up Python Environment (using `uv`):**
    It is highly recommended to use a virtual environment.
    bash
    # Install uv if you don't have it
    # curl -LsSf https://github.com/astral-sh/uv/releases/latest/download/install.sh | sh

    # Create a virtual environment and activate it
    python -m venv .venv
    source .venv/bin/activate  # On Windows use `.venv\Scripts\activate`

    # Install dependencies using uv
    uv install
    

3.  **Run Linters and Formatters:**
    bash
    ruff check
    ruff format
    

4.  **Run Tests:**
    bash
    pytest
    

## 5. Contribution Guidelines

*   **Code Quality:** Adhere to PEP 8 standards and the linting rules enforced by Ruff.
*   **Readability:** Write clear, concise, and well-documented code.
*   **Modularity:** Design code with modularity and reusability in mind.
*   **Testing:** Ensure all new code is accompanied by relevant tests.
*   **API Design:** Follow FastAPI best practices for routing, request validation, and response modeling.
*   **AI Integration:** If modifying AI-related components, ensure API keys are handled securely (e.g., via environment variables) and that interactions with AI models are robust and efficient.

## 6. Getting Help

If you have questions about contributing or the project's architecture, please open an issue. We strive to maintain a supportive and collaborative environment.
