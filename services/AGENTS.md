
# Module Context

Handles all communication with Google Gemini models for text analysis, copywriting, and image generation for "모두의 상세페이지".

# Tech Stack & Constraints

- Models: gemini-3-flash-preview (Text), gemini-3-pro-image-preview (Image).
- Libraries: @google/genai.
- Constraints: Images must be processed as base64 strings with correct IANA MIME types.

# Implementation Patterns

- **Retry Logic:** Use exponential backoff for 429 and 503 errors.
- **JSON Parsing:** Always clean markdown wrappers (```json) before parsing response.text.
- **Tone & Manner:** When generating images, use reference images only for style/lighting cues, never content duplication.

# Testing Strategy

- Connectivity Check: performDeepConnectionTest for latency and model availability.

# Local Golden Rules

- **Do's:** Extract URLs from groundingChunks if using Google Search/Maps grounding.
- **Don'ts:** Do not call .text() as a method; access the .text property directly.
