# Planning safety certificate

↑ **Parent:** [Formal specification](formal-specification.md)

An auxiliary [planning fluent](planning-fluent.md) certifying that a safety condition has been checked for the current state in [automated planning](automated-planning.md). A checking action requires facts establishing the condition and adds the certificate; the hazardous action requires that certificate.

Every action capable of invalidating the check must delete the certificate. Otherwise checking a safe configuration and then changing it could authorize an unsafe action using stale evidence. For river crossing, certify that the departure bank contains no incompatible pair, invalidate the certificate on every load, unload or crossing, and require it before sailing. This compiles a safety test into positive [STRIPS](strips.md) [preconditions](precondition.md) when a suitable finite static compatibility relation is supplied.

## ↑ Ancestors (6)

1. [Formal specification](formal-specification.md)
2. [Formal verification](formal-verification.md)
3. [Algorithm correctness](algorithm-correctness.md)
4. [Algorithm](algorithm-split.md)
5. [Computer science](computer-science-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-computer-science-course-of-the-university-of-oxford/2023/artificial-intelligence/2/g/solution.md)
