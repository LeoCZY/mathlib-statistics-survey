---
title: "TITLE"
source_module: "LEAN_MODULE"
source_path: "LEAN_FILE"
mathlib_commit: "COMMIT"
last_update: "DATE"
topics:
  - "TOPIC"
---

# TITLE

Mathlib source: [LEAN_MODULE](SOURCE_LINK)

Companion Lean file: [CHECKS_FILE](CHECKS_FILE)

The goal is to explain clearly all mathematics in the fixed Lean file and how
the Lean code expresses it. Delete questions that are not useful for the file.

## 1. Mathematical result and Lean translation

- What is the main theorem or definition?
- What does it say in ordinary mathematics?
- What is its exact Lean statement?
- What assumptions or implicit arguments appear in Lean?
- What does the initial tactic state show?

### Main result

**Mathematics.**

*State the result here.*

**Lean.**

```lean
-- Exact source declaration
```

```lean
#check DECLARATION_NAME
```

```text
Infoview output
```

### Proof

- What is the mathematical proof?
- How does each important Lean line correspond to a mathematical step?
- What formula or goal does Infoview show at that step?

**Mathematical proof.**

*Write the proof here.*

**Lean proof.**

```lean
-- Exact proof from the fixed source
```

*Explain a proof line only when the math–Lean correspondence is not obvious.*

## 2. Core definitions

- Which definitions are needed to understand the main result?
- What is the mathematical formula for each definition?
- How is it written in Lean?
- Which existing `#check` prints the formula?

Repeat this block for each definition.

### Definition N: NAME

**Mathematics.**

*Write the definition and formula here.*

**Lean.**

```lean
-- Exact source definition
```

**Infoview.**

```lean
#check DEFINITION_OR_BRIDGE_THEOREM
```

```text
Infoview output
```

## 3. Other public declarations

- What other mathematical declarations are defined in the file?
- What does each one say mathematically?
- Why is it useful?
- Does its proof or Lean design contain something worth explaining?

| Mathematical role | Lean declaration |
| --- | --- |
| ROLE | `DECLARATION` |

## 4. Boundary conditions

- How does the code deal with boundary conditions?
- How does its scope differ from a cited source?

Write only what is present in the source. If there is no meaningful boundary case,
say so briefly.

## 5. Discussion
- what are next steps?
- Anything else you wanna discuss?

## 6. References

- Which book, paper, documentation page, issue, or pull request is relevant?
- Chek over Foundations of Modern Probability https://link.springer.com/book/10.1007/978-3-030-61871-1
