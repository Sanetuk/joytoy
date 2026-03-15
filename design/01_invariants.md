# System Invariants

This document defines rules that must never be violated by implementations.

If any rule conflicts with code or design interpretation,
the invariant is authoritative.

---

## Layer Separation

Extraction, Transfer, and Conversion are independent layers.

Extraction MUST NOT:
- perform logistics transfer
- perform industrial conversion

Transfer MUST NOT:
- generate resources
- transform resources

Conversion MUST NOT:
- directly interact with natural sources

---

## Authority of Nodes

Field Cache is not a logistics authority node.

Only Depot may act as a stable logistics endpoint.

Implementations MUST NOT treat field caches as depots.

---

## Network Logic

A logistics network is established only when a persistent transfer
relationship exists between nodes.

A single movement of goods does not constitute a logistics network.

---

## Catalog Integrity

Codex agents MUST NOT invent:

- new buildings
- new services
- new node types
- new item families

If a required element is missing, return:

UNSPECIFIED

---

## Knowledge vs Goods

Knowledge payloads are informational outputs.

They MUST NOT be treated as:

- logistics cargo
- industrial material
- tradable physical goods

---

## Ontology Protection

Implementations MUST NOT modify the ontology of the system.

Forbidden actions include:

- redefining glossary terms
- changing layer meanings
- introducing new system layers

Ontology changes require human design approval.