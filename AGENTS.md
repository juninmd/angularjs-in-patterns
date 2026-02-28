```markdown
# AGENTS.md - Guidelines for AI Coding Agents

These guidelines are designed to ensure consistent, maintainable, and high-quality code for our AI coding agents. Adherence to these principles is crucial for a successful and reliable development process.

## 1. DRY (Don't Repeat Yourself)

*   All logic, data processing, and API interactions must be encapsulated within reusable functions, classes, or modules.
*   Avoid duplication of code; refactor existing code to create single, cohesive units.
*   Document functions and classes thoroughly, explaining their purpose, inputs, and outputs.
*   Prioritize code modularity and abstraction.

## 2. KISS (Keep It Simple, Stupid)

*   Strive for minimal code complexity.
*   Use straightforward and understandable constructs.
*   Avoid overly clever or convoluted solutions.
*   Prioritize readability and clarity.

## 3. SOLID Principles

*   **Single Responsibility Principle:** Each class/module should have one primary responsibility.
*   **Open/Closed Principle:**  The system should be extensible without modifying the core implementation.  New functionality should be added through new classes/modules, not by modifying the existing ones.
*   **Liskov Substitution Principle:**  Subclasses should be substitutable for their base classes without altering the correctness of the program.
*   **Interface Segregation Principle:** Client code should not be forced to depend on methods it does not use.
*   **Dependency Inversion Principle:** High-level modules (like agents) should not depend on low-level modules (like data structures).

## 4. YAGNI (You Aren't Gonna Need It)

*   Only implement functionality that is currently required and expected.
*   Avoid adding features or code that is not explicitly needed at this time.
*   Refactor and simplify existing code to eliminate unnecessary elements.

## 5. Development Focus & Productivity

*   All development must be productive; do not introduce distractions.
*   Focus on delivering working code first.
*   Prioritize testing, validating assumptions and proper data handling.
*   Ensure all code completion and suggestions are valuable and align with current requirements.
*   Implement robust error handling and logging.

## 6. Code Length & Structure

*   Maximum code length: 180 lines.
*   Structure:  Clearly organized with consistent indentation and spacing.
*   Comments:  Use comments sparingly and only to explain *why* not *what*.  Focus on technical understanding.
*   Documentation:  Include detailed docstrings for each function/class/module explaining its purpose, parameters, return values, and potential side effects.

## 7. Testing

*   All code must be thoroughly tested.
*   Unit tests should cover all critical functionalities.
*   Test cases should be written *before* implementation, utilizing existing mocks.
*   Automated testing should be included.
*   Test coverage:  Aim for at least 80%.

## 8. Data Handling

*   Use appropriate data structures (lists, dictionaries, etc.) to represent data efficiently.
*   Handle data gracefully in case of errors or unexpected inputs.
*   Document data structures and their use clearly.
*   Avoid complex data transformations unless absolutely necessary.

## 9. Dependencies

*   Dependencies should be clearly defined and documented.
*   Manage dependencies using a version control system.
*   Consider dependency injection to improve testability and maintainability.

## 10. AI-Specific Considerations

*   Design agents with clear input/output expectations.
*   Implement efficient data processing logic.
*   Utilize appropriate data structures for agent state management.
*   Prioritize algorithmic efficiency.

## 11.  File Structure (Example)

```
AGENTS.md
├── __init__.py
├── agents.py          # Core logic and data structures
├── utils.py           # Utility functions
├── data_processing.py  # Data manipulation logic
├── error_handling.py   # Error management and logging
└── tests/            # Test suite
    ├── test_agents.py
    └── ...
```

These guidelines are subject to change and refinement as the AGENTS project evolves.  Any modification requires formal review and approval from the team.
```