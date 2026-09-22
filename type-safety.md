# Type safety

↑ **Parent:** [Type system](type-system.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Type_safety)

For a specified [programming language](programming-language-split.md) and execution model, [type safety](type-safety.md) commonly follows from two properties: a closed expression satisfying a [typing judgment](typing-judgment.md) is either a value or can take an execution step, and taking a step preserves its type. Proofs proceed by [structural induction](structural-induction.md) on derivations, using [capture-avoiding substitution](capture-avoiding-substitution.md) for function calls. Repeated preservation keeps the remaining expression typed; the first property then rules out getting stuck at an operation outside the model's permitted cases. This argument does not imply termination or correctness of an arbitrary specification. [Software Foundations, Programming Language Foundations, Type Systems: progress, preservation and type soundness](https://softwarefoundations.cis.upenn.edu/plf-current/Types.html)

## ↑ Ancestors (4)

1. [Type system](type-system.md)
2. [Programming language](programming-language-split.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Type safety](type-safety.md)
- [Type system](type-system.md)
