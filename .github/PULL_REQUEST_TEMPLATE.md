# Pull Request Template

## 1. PR Overview

**Title:** (Concise and descriptive title for your changes)

**Description:**

*   **What was changed?** (Briefly summarize the core purpose and scope of this PR.)
*   **Why was it changed?** (Explain the motivation behind these changes. Link to issues if applicable.)
*   **How was it changed?** (Describe the approach taken to implement the changes.)

---

## 2. Checklist

Before submitting your Pull Request, please ensure:

*   [ ] **Code Style & Linting:** Code adheres to project standards. All files have been formatted (e.g., using Ruff).
*   [ ] **Unit Tests:** New or modified functionality is covered by comprehensive unit tests.
*   [ ] **Integration Tests:** If applicable, integration tests have been updated or added.
*   [ ] **Documentation:** Relevant documentation (code comments, README sections) has been updated.
*   [ ] **Dependencies:** Any new dependencies are justified and added correctly to `pyproject.toml`.
*   [ ] **CI/CD:** All GitHub Actions checks (CI, linting, testing) pass.
*   [ ] **Security:** No introduction of known security vulnerabilities.

---

## 3. Related Issues

*   Closes # (If this PR resolves a specific issue, link it here using `Closes #<issue-number>`)
*   Relates to # (If this PR is related to another issue but doesn't fully close it.)

---

## 4. Architectural Alignment

*   **Apex Principles:** This PR aligns with the Apex Technical Authority's philosophy of "Zero-Defect, High-Velocity, Future-Proof."
*   **Tech Stack:** Changes are consistent with the Python 3.10+ stack using uv, Ruff, and Pytest.
*   **Architecture:** The changes adhere to the **Modular Monolith** pattern, maintaining clear separation of concerns.

---

## 5. Testing & Verification

*   **Testing Strategy:** All changes have been verified locally using the following commands:
    bash
    # Example commands - adapt as needed for specific tests
    uv run pytest tests/
    uv run ruff format .
    uv run ruff check .
    
*   **Verification Steps:** (Optional) Provide any specific steps required to manually verify the changes.

---

## 6. Additional Notes

(Any other relevant information, screenshots, or context you'd like to provide.)
