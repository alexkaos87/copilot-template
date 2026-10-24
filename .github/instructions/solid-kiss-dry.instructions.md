---
applyTo: **
description: "Use when designing, implementing, refactoring, or reviewing code. Apply SOLID principles, Keep It Simple, Stupid (KISS), and Don't Repeat Yourself (DRY) pragmatically."
version: 1.0.0
excludeAgent: false
---

# Practical Design Principles

- **SOLID:** Give each type or module a clear responsibility; extend behavior without needlessly modifying stable code; depend on small abstractions at genuine boundaries; and keep interfaces focused. Use substitutable implementations where polymorphism is intended. Do not introduce interfaces, inheritance, or indirection without a concrete need.
- **KISS (Keep It Simple, Stupid):** Prefer the clearest solution that meets the requirements. Avoid speculative features, premature optimization, unnecessary layers, and clever constructs that make behavior harder to understand.
- **DRY (Don't Repeat Yourself):** Keep one authoritative implementation for the same business rule or knowledge. Extract shared logic when duplication is real and likely to change together; do not couple unrelated code just because it looks similar.
- Preserve existing behavior and follow established project patterns unless there is a clear reason to change them.
- Prefer small, cohesive changes. Add tests for meaningful behavior and edge cases, and avoid abstractions that make the code harder to use or verify.
