# Week 8 AI Presenter Prototype and Validation
Student: Kevin Eloi
Date: 11/2/26
Branch: feature/week-8-avatar-prototype
HeyGen project: CampusConnect Welcome - Eloi
## 1. Prototype hypothesis
If a short AI presenter explains the chatbot's scope, privacy boundary, and
human fallback before the first question, a new user will understand how to
begin without making the text path harder to use.
## 2. Required prototype behavior
- The presenter is a HeyGen public stock avatar, not an impersonation or clone.
- The visible disclosure says the presenter is AI-generated.
- The video does not autoplay.
- A complete transcript is visible without playing the video.
- The existing text chatbot remains usable if the video is paused, muted,
 blocked, slow, or ignored.
- The script contains no real student, employee, or institutional private data.
- The original local RAG grounding, citations, abstention, and human fallback
 remain unchanged.
## 3. Five-test record
| # | Test | Expected behavior | Observed result | Pass / Revise |
|---|---|---|---|---|
| 1 | Open the page but do not play the video. | AI disclosure and transcript are visible. | <FILL IN> | <FILL IN> |
| 2 | Play the presenter once. | It is 30-60 seconds and states scope, privacy, and fallback. | <FILL IN> | <FILL IN> |
| 3 | Mute or pause the video. | The transcript and text chatbot still communicate the essential information. | <FILL IN> | <FILL IN> |
| 4 | Ask: How do I reset my CampusConnect password? | The existing RAG answer and source citation still work. | <FILL IN> | <FILL IN> |
| 5 | Ask: What are the Thanksgiving dining hall hours? | The chatbot abstains or gives a safe human next step. | <FILL IN> |<FILL IN> |
## 4. One design decision
- Evidence I observed:
- Decision: KEEP / CHANGE / REMOVE the presenter path
- One reason:
- One small revision made:
## 5. Engineering and AI Use Log
- AI tools used: HeyGen and ChatGPT
- What HeyGen generated:
- What ChatGPT changed in app.py:
- What I verified myself:
- Remaining limitation:
