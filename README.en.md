# Ramble to Clarity

A skill that turns free-form speech transcripts, brain dumps, and scattered notes into a faithful intent brief and a useful outline, draft, decision frame, or action plan.

[中文说明](README.md)

## Use cases

Use it when you have context but have not organized it yet, want to think aloud before choosing a direction, or need to clarify motivations and constraints before writing or planning. Input can be one message, multiple conversational turns, or an existing transcript. There is no required speaking duration. The skill itself does not record or transcribe audio.

## Workflow

| Phase | Behavior |
| --- | --- |
| Collect | Let the user continue without premature synthesis. |
| Reflect | Reconstruct the goal, motivations, constraints, and open questions. |
| Clarify | Ask only questions that materially affect the result. |
| Deliver | Produce the brief, outline, draft, decision frame, or plan the user needs. |

The workflow is flexible. A clear request with enough context can proceed directly to a deliverable.

## Installation

The repository root is the skill directory. `SKILL.md` is the only required file. For Codex, copy the directory as `ramble-to-clarity` under your personal skills directory:

```text
~/.codex/skills/ramble-to-clarity/SKILL.md
```

When `CODEX_HOME` is set, use `skills/ramble-to-clarity` under that directory. For other tools that support skill files, follow their installation instructions. Compatibility has not been tested across every host.

## Example requests

```text
$ramble-to-clarity
I will send several chunks. Wait until I am finished before organizing them.
```

Then:

```text
I am finished. Reflect the problem I am trying to solve, my constraints, and the parts that remain unclear.
```

For writing:

```text
$ramble-to-clarity
Turn the transcript below into an article outline for beginners. Preserve my central position and flag claims that need verification.
```

## Attribution and limitations

Inspired by [Andrej Karpathy's X post](https://x.com/karpathy/status/2079610838143623371). The post describes a personal working habit. This repository's phases, output fields, and quality checks are additional design choices, not an official Karpathy methodology.

The skill can still misunderstand the user. Check important constraints and conclusions. External factual accuracy depends on available sources and verification tools. The package passed structural validation; it has not undergone broad user testing.

## Publishing

This directory can be uploaded as a GitHub repository. It includes no personal paths, account credentials, or dependency on a particular voice product. An open-source license has not been selected; add one according to your publishing intent.
