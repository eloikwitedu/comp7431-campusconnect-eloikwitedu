# CampusConnect Requirements Specification v1
Status: Draft — Week 3
Student: Kevin Eloi
Branch: docs/week-3-requirements-ai

## 1. Problem statement
Students who need IT Support information need a reliable way to find the correct 
next step because the current experience may be scattered, difficult to search, or 
hard to verify as current.

## 2. Evidence carried forward from Week 2
- E-01: Documentation is fragmented and tickets submitted are often vague.
- E-02: Though the desk help worker sees the ticket status, they are unsure how a department handled it.
- A-01: We assume students would find a short answer linked to approved IT Support material useful.

## 3. One user journey inside the MVP
A student asks one typed IT Support question. CampusConnect searches only approved 
IT Support material, returns a short answer with a visible source, or says the 
available sources do not support an answer.

## 4. Four requirements
- FR-01 — The system shall accept one typed IT Support question.
- GR-01 — Every factual answer shall identify the approved source used.
- SF-01 — If approved sources are insufficient, the system shall not invent an 
answer and shall provide a helpful IT Support next step.
- NFR-01 — A keyboard user shall be able to submit a question and read the result.

## 5. MVP boundary
IN: one typed question, approved IT Support material, one grounded answer, visible 
source, safe failure, and helpful next step.
OUT: password resets, ticket creation, personal student records, voice, automatic 
actions, and answers from unapproved material.

## 6. AI critique and human decision
- ChatGPT suggestion: Revise GR-01 so the cited approved source must support the answer, rather than merely be named.
- Claude suggestion: Make SF-01’s rule for when to withhold an answer testable using questions with and without support in approved sources.
- My decision: Accepted (Claude)
- My reason: This allows for SF-01 to have a more testable guideline for what an insufficient source is to see whether or not CampusConnect correctly answers or withholds.
