# Canonical Glossary (Authority Terms)

This document defines canonical meanings of core system terms.
Codex agents MUST NOT reinterpret or extend these definitions.

If a term is not defined here, treat it as UNSPECIFIED.

---

## Core Layers

### Extraction
Services that turn **natural sources** into **available materials**.

Extraction:
- interacts with natural deposits or biological sources
- produces raw or minimally processed materials

Extraction DOES NOT:
- move goods through networks
- perform industrial transformation

---

### Transfer
Services that move goods between nodes.

Transfer:
- establishes logistics connections
- creates persistent supply relationships

Transfer DOES NOT:
- create goods
- transform goods

---

### Conversion
Services that transform goods into other goods.

Conversion:
- applies recipes or industrial processes
- consumes inputs and produces outputs

Conversion DOES NOT:
- extract natural resources
- provide long-distance logistics

---

## Node Types

### Field Cache
A temporary staging point.

Field Cache:
- stores goods temporarily
- may support expeditions

Field Cache DOES NOT:
- serve as authoritative logistics hub
- replace a depot

---

### Depot
Authoritative logistics node.

Depot:
- acts as official transfer endpoint
- stabilizes logistics networks

Depot DOES NOT:
- perform general industrial conversion

---

### Provisional Factory
Temporary industrial node.

Provisional Factory:
- performs limited conversion
- usually batch-based

Provisional Factory DOES NOT:
- represent permanent industrial infrastructure

---

## Knowledge

### Knowledge Payload
Information produced by analysis activities.

Knowledge payload:
- is informational output
- is not a physical good
- is not transported as logistics cargo

---

## Rule for Undefined Terms

If implementation requires a concept not present in this glossary:

Return:

UNSPECIFIED

Do NOT invent new canonical terms.