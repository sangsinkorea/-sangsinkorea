
# Project Context & Operations

모두의 상세페이지: AI-powered e-commerce detail page and thumbnail generation system.
Tech Stack: React, Tailwind CSS, @google/genai SDK, jsPDF.

Operational Commands:
- Local Development: npm run dev
- Build: npm run build

# Golden Rules

- **Immutable (Strict Compliance):** Only implement features explicitly requested by the user. Do not add unasked functionality or content to the code.
- **Proactive Suggestion:** Propose enhancements or extra features in natural language only. Never implement them without direct confirmation.
- **Security:** Use process.env.API_KEY exclusively. No hardcoded keys or user-facing key management UI except through authorized system dialogs.
- **Scale:** Maintain all AGENTS.md files under 500 lines.
- **Formatting:** No emojis allowed in rules or implementation logic to preserve context efficiency.

# Standards & References

- Coding Convention: Functional React components with TypeScript.
- Image Aspect Ratios: 9:16 for detail sections, 1:1 for thumbnails.
- Maintenance: If instructions and code conflict, suggest a rule update immediately.

# Context Map (Action-Based Routing)

- **[Global Logic & Entry](./App.tsx)** — Main application state and tab switching.
- **[Gemini API Services Logic](./services/AGENTS.md)** — All GenAI SDK interactions and prompt engineering.
- **[UI Component Architecture](./components/AGENTS.md)** — Feature-specific UI logic and rendering flows.
- **[Shared Data Structures](./types.ts)** — Core interfaces and type definitions.
