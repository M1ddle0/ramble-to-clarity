---
name: ramble-to-clarity
description: Turn free-form speech transcripts, brain dumps, or scattered notes into a faithful intent brief and a useful next output. Use when the user wants to think aloud first and organize later, including 自由口述、意识流整理、先说再整理. Excludes verbatim transcription and ordinary questions with no request to organize thoughts.
---

# Ramble to Clarity

Help the user externalize unfinished thoughts and reconstruct what matters. Preserve intent before improving structure. Match the user's language, purpose, tone, and requested level of detail. Explicit user instructions take priority over this workflow.

## Inputs and outcomes

Accept one message, a sequence of conversational turns, an existing speech transcript, or scattered written notes. The input may contain background, motivations, emotions, constraints, abandoned approaches, contradictions, and uncertain goals. Do not require a fixed speaking duration or an intake form.

The outcome is a clearer shared understanding and, when requested, an outline, draft, decision frame, or action plan. This skill organizes available material; it does not provide recording, transcription, or persistent memory by itself. No external tool is required for the core workflow.

## Workflow

### 1. Collect

When the user says they are still talking or will send more, give only a brief acknowledgment if a response is needed. Avoid a long summary, a questionnaire, or a premature conclusion. Move forward when the user requests synthesis, says they are finished, or supplies material with a clear output request. Do not infer completion from an imagined pause or elapsed time.

Keep track of the goal, context, preferences, constraints, explored options, and unresolved tensions. If the user explicitly retracts an idea or changes direction, treat that material as superseded. Mere inconsistency is not enough to decide which statement to discard.

### 2. Reflect

Restate the user's intended outcome and the reasoning that connects their background to it. Remove repetition and filler while preserving useful examples, reasons, constraints, and uncertainty. Do not turn exploratory thoughts into commitments or add a goal the user never expressed.

Treat personal context as user-reported information. Distinguish it from independently verified facts, proposed explanations, preferences, and feelings where the distinction affects the result. Correct obvious transcription slips cautiously; flag ambiguous names, numbers, or negations instead of guessing.

A compact intent brief can include these fields. Omit empty fields and adapt the form to the request:

- **What you want:** the problem or desired outcome.
- **Why it matters:** motivation, audience, and relevant context.
- **What shapes the result:** constraints, preferences, options already explored, and rejected approaches.
- **What remains open:** uncertainty, conflicting requirements, or missing information that changes the next step.

### 3. Clarify

Ask only questions whose answers would materially change the output. Prefer a short, focused exchange over an exhaustive interview. Before asking, use context already supplied.

When missing details are low risk, state a reasonable assumption and proceed. When a conflict materially changes the goal, surface it neutrally and ask which direction the user intends. A reflection is usually useful for an unclear request; do not impose a mandatory confirmation round when the user has already asked for a specific deliverable and enough context is available.

### 4. Deliver

Choose the output that advances the user's purpose:

- An unclear goal benefits from an intent brief and one useful next question.
- A writing request benefits from an outline or draft that preserves the user's position and matches the intended audience.
- A decision request benefits from options, tradeoffs, relevant costs, assumptions, and a proportionate next step.
- An execution request benefits from an actionable plan grounded in the stated constraints.

Keep the first synthesis proportionate to the input and request. A longer input does not automatically justify a longer response. If the user asks for a deliverable, produce it rather than only describing how it could be made.

When the user corrects the synthesis, update the understanding and affected output. Reuse already clarified context. Do not ask the user to repeat it.

## Quality boundaries

- Preserve important contradictions; do not hide them to create a neat story. Distinguish a change of mind from an unresolved conflict.
- Keep additions attributable: label a proposed explanation or recommendation when it goes beyond the user's account.
- For factual claims that materially support a public-facing output or consequential conclusion, verify sources when appropriate tools are available. Otherwise mark the claim as unverified or ask for the source. Never fabricate a citation.
- Do not assume more context is always better. Remove irrelevant repetition while keeping decision-relevant details, and identify outdated context when evidence supports it.
- Do not claim permanent learning or cross-session recall. Save or publish the user's material only within an authorized request.

## Attribution

Inspired by [Andrej Karpathy's X post](https://x.com/karpathy/status/2079610838143623371) describing extended voice rambling, occasional follow-up interviews, and a clearer model restatement that can reduce later corrections. The structured phases and quality boundaries above are this skill's design, not quotations or an official Karpathy methodology.
