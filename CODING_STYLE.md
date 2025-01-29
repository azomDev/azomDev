# Personal Programming Specification

This document outlines my personal coding style and philosophy, explaining the reasoning behind my choices.

## Indentation & Spacing
I use **tabs** for indentation. The primary reason is that tabs allow each coder to configure their own preferred spacing, making it adaptable to different visual preferences and font settings. This enhances readability across various setups without enforcing a fixed width.

## Naming Conventions
Consistent naming conventions help with readability and maintainability. My preferred conventions are:
- **Variables**: `snake_case` - Improves readability, especially in languages that use underscores frequently.
- **Functions**: `camelCase` - A common convention in many languages, making function names stand out.
- **Classes**: `PascalCase` - Differentiates class names from other identifiers.
- **Constants**: `SCREAMING_CASE` - This ensures that constants are visually distinct.

## Commenting & Documentation
There is no strictly defined approach to documentation. The preferred style depends on the **language** and **team** working on the codebase. The focus should be on clarity and keeping documentation useful rather than enforcing a rigid format.

## Code Structure & Organization
Code should be structured in a way that is **balanced**—neither deeply nested nor overly flat. A well-organized structure ensures:
- Files are easy to locate without excessive directory navigation.
- The overall layout is intuitive for new developers entering the codebase.

## Line Length & Wrapping
There is no strict line length preference—it depends on the language and community standards. However, I may define more specific wrapping rules in the future.

## Error Handling
The choice of error-handling method depends on the language. However, for more **robust** code, it is generally preferable to return error values rather than throwing exceptions (as seen in languages like Rust). This approach ensures that even without documentation, when calling a function from elsewhere, it is immediately clear that it can return an error, rather than potentially encountering an exception thrown deeply in the stack, which may not always be specified in the documentation.

**TODO:** Expand on this section with more detailed best practices.

## Code Style Enforcement
Use of linters and formatters depends on the language and available tools. There is no one-size-fits-all enforcement; it remains a personal preference per project.

## Dependencies & Third-Party Libraries
Before adding a dependency, consider:
- Whether the needed functionality can be implemented with a small amount of code instead of adding a dependency. Adding unnecessary dependencies increases complexity and potential points of failure.
- More dependencies introduce **more points of failure** and can increase complexity for newcomers. Thoughtful selection is key.

## Version Control & Commits
No strict commit message style is enforced. Developers are free to use their preferred style. Similarly, there are no rigid policies on squashing commits or branching strategies—it depends on the team and project requirements.

---
This document serves as a guide for my coding preferences. It may evolve over time as I refine my approaches based on experience and collaboration.

