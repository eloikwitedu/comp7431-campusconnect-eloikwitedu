# Week 10 MVP Test, CI, and Freeze
Student: Kevin Eloi
Date: 11/16/26
Branch: release/week-10-rc1
Local URL: http://127.0.0.1:7860
Environment: Chrome on macOS
## 1. Six-test MVP record
| # | Quality area | Action and expected result | Observed evidence | Result |
|---|---|---|---|---|
| 1 | Supported retrieval | Ask: "How do I reset my CampusConnect password?" The answer uses the approved password-reset passage. | Source: IT-01 — Password reset | PASS |
| 2 | Citation support | Open the displayed source from Test 1. At least one important answer claim is directly supported by the source passage. | The agent instructed the user about the password reset workflow closely | PASS |
| 3 | Unsupported query | Ask: "What are the Thanksgiving dining hall hours?" The system states its IT-support limit and does not invent hours, a source, phone number, or office. | The approved guide doesn't support an answer to this question. | PASS |
| 4 | Voice and text fallback | Use the supported answer. If voice works, its meaning matches the visible grounded answer. If voice is unavailable, the text, source, and a clear Continue in text or retry path remain. | The meaning matched with the text based response and RAG documents | PASS |
| 5 | Video accessibility | Mute the tab and skip the video. AI disclosure and transcript remain visible, and the chatbot is reachable by keyboard. | The video is accessible via closed captions | PASS |
| 6 | Latency and recovery | Time one supported question. Class target: grounded text in 5 seconds or less. If slower, the question is preserved and progress, retry, or text fallback is clear. | The grounded results were returned within milliseconds | PASS |
## 2. Lighthouse and manual accessibility evidence
Performance score: 97
Accessibility score: 100
One important Lighthouse finding or "none listed": Server responded slowly
Keyboard plus muted-video result: Keyboard Accessibility PASS
## 3. Defect decision and retest
Highest-severity finding: None
Severity: NONE
Smallest repair made: No repair required
Focused retest result: N/A
## 4. Release gate
Release decision: Go
Decision reason: No severe findings
GitHub Actions run: <PASTE RUN URL>
Release tag if GO: v0.9.0-rc1
## 5. Engineering and AI Use Log
What I tested myself: Accessibility
What remained human-reviewed rather than automated: Visual overview
Known limitation carried into Week 11 Red Teaming: Pressing the agent about unsupported evidence
