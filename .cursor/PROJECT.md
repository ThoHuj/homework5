# Homework 5 — /sync Slash Command

## Goals

- Implement a Cursor slash command (`/sync`) that forces the agent to pause and self-evaluate.

## Process

- Commands live in `.cursor/commands/` as markdown files.
- All command text in English.
- Evidence lines in `/sync` responses must be at most 80 characters.

## Specification

- `/sync` must stop current work before answering.
- Response follows the fixed 5-part template (goal, process, spec, momentum, next step).
- Each evidence field includes a concrete, short proof (≤ 80 chars).
- Stuck detection: agent flags loops, useless steps, or confirms on-track progress.
