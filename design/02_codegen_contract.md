# Codex Implementation Contract

This document defines how Codex agents must behave when working on this repository.

Before starting any implementation task, the agent MUST read:

1. design/00_canonical_glossary.md
2. design/01_invariants.md

These documents are authoritative.

---

## Authority Order

The following precedence must be respected:

1. invariants
2. glossary
3. repository source code
4. implementation details

If conflicts occur, higher authority wins.

---

## Allowed Decisions (Green Zone)

Codex may decide:

- internal code structure
- function naming
- module organization
- algorithm implementation

As long as invariants are respected.

---

## Conditional Decisions (Yellow Zone)

Codex may create placeholders when information is missing.

Allowed placeholders include:

UNSPECIFIED
TODO
PLACEHOLDER

These indicate missing design information.

---

## Forbidden Decisions (Red Zone)

Codex MUST NOT:

- invent new game content
- invent new buildings
- invent new node types
- invent new services
- redefine glossary terms

If required data is missing, return UNSPECIFIED.

---

## Catalog Safety Rule

Concrete game content must come from canonical sources only.

Examples of concrete content:

- buildings
- services
- recipes
- item definitions

If not defined in source documents,
the agent must not fabricate them.

---

## Self-Audit Requirement

Before completing any task, the agent must check:

1. Did I introduce new ontology terms?
2. Did I reinterpret glossary definitions?
3. Did I invent catalog content?

If any answer is YES, the implementation is invalid.

The agent must revise the result.

---

## Implementation Philosophy

The system prioritizes ontology stability over implementation speed.

It is preferable to return UNSPECIFIED rather than introduce incorrect concepts.