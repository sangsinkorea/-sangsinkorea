
# Module Context

UI components for product input, detail page planning, and thumbnail generation for "모두의 상세페이지".

# Tech Stack & Constraints

- Styling: Tailwind CSS.
- PDF Export: jsPDF (A4/E-commerce vertical formats).
- State Management: React useState and useRef.

# Implementation Patterns

- **Step-based Workflow:** INPUT -> PLANNING -> REVIEW -> GENERATING -> RESULT.
- **Visual Feedback:** Provide real-time rendering logs (e.g., "AI Artist: Sketching layout...") during generation.
- **Sticky UI:** Use sticky headers for control panels during the review phase.

# Local Golden Rules

- **Do's:** Ensure all sections have a 'Retry' or 'Individual Generation' button.
- **Don'ts:** Do not modify the prompt-generated copywriting unless requested by the user.
