# cursor-rules

## Setup Instructions

To implement this Standard Operating Procedure (SOP) in your AI IDE (Cursor, Windsurf, Antigravity, etc.):

1. **Global Rules**: Open your IDE settings (e.g., Cursor Settings -> Rules and Commands -> User Rules) and paste the entire content of `cursorrules.txt`. These rules are tuned for small, cost-efficient models like GPT-5.1 mini/nano, so pair this step with a tiny model for the biggest savings.
2. **Workspace Folder**: Copy the `rules/` folder from this repository into the root of your project workspace. Maintain the directory structure (`rules/mvp/` and `rules/production/`).
3. **Repository Hygiene**: Ensure your project has the `.gitignore` and `.cursorignore` files provided in this repository to prevent the AI from processing unnecessary files.

## Assumptions
- **User Initiative**: It is assumed the user will proactively select a mode (`[MVP]` or `[Production]`) at the start of a task.
- **Project Structure**: It is assumed the project follows a standard layout where the `rules/` folder can reside at the root.
- **Model Agnostic**: These rules are designed to work across various LLMs, though performance may vary slightly between models.

## Trade-offs
- **Speed vs. Precision**: Writing an Enhanced Task Brief (ETB) before coding adds a small upfront time cost but prevents expensive "generate → error → retry" loops.
- **Strictness vs. Flexibility**: The "No code before approval" rule enforces rigor at the cost of immediate execution.
- **Context Management**: Using `.cursorignore` saves significant tokens and costs but requires manual updates if new critical directories are added.
