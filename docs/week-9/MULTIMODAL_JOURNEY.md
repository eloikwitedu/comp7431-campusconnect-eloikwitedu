# Lab09 Multimodal Journey Evidence
Branch: feature/week-9-multimodal-integration
## Journey A — Supported
- Input method used: VOICE
- RAG answer observed: Noted that it does not have access to documentation for password reset
- Citation or source observed: N/A
- Voice behavior: It responded with voice correctly
- Video remained optional: REVISE
## Journey B — Unsupported
- Question used: How many 'r's are in the word "strawberry"?
- Abstention or human next step observed: The chatbot responded and answered instead of focusing on the CampusConnect system.
- Text fallback worked with video muted/skipped: YES
## Traceability
- Requirement: one optional multimodal CampusConnect journey
- Files changed:
src/styles.css
src/routes/__root.tsx
src/routes/index.tsx
src/components/ui/button.tsx (stronger keyboard focus outline, video-area button style)
src/components/campus/TextAsk.tsx (new)
src/components/campus/VoiceCard.tsx (new)
src/components/campus/VideoCard.tsx (new)
src/lib/campus-guide.ts (new)
src/lib/campus-guide.test.ts (new)
src/types/elevenlabs.d.ts (new)
AGENTS.md
- Known limitation:
