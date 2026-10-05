# Week 4 LM Studio RAG Results
Name: Kevin Eloi
Model: IBM Granite 4.0 H Tiny Q4_K_M
Documents: campusconnect password help.txt, campusconnect wifi help.txt

## Supported question
Result: PASS
Observation: It noted to include the device type, the exact error message displayed, and the time it occurred. It sourced only the wifi help file.

## Unsupported question
Result: PASS
Observation: It said there was not enough approved evidence to support, saying no information exists on purchasing a laptop or reimbursements. It suggested to contact the Business Office directly.

## Action request
Result: PASS
Observation: It requested I reach out directly to CampusConnect IT, noting it does not have enough approved evidence to support with no information on how to perform a password reset.

## Architecture lesson
The local LLM route worked well when files directly related to the question asked. It needs human help when questions were vague or outside the bounds of what was provided.
