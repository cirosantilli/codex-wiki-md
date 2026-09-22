# Semigroup simulation of a Turing machine

↑ **Parent:** [Finite semigroup presentation](finite-semigroup-presentation.md)

A finite deterministic [Turing machine](turing-machine.md) can be represented by a [finite semigroup presentation](finite-semigroup-presentation.md) whose generators are tape symbols, state symbols, a boundary marker $h$, and an accept symbol $q$. Defining equalities replace the local scanned symbol and state according to machine instructions, with separate boundary cases for implicit blanks. Only terminal-state equalities erase tape letters and then replace $hq_Hh$ by $q$. A derivation from an initial description to $q$ must encounter a terminal state before its first erasure. Simulation equalities preserve halting membership in either direction: for a deterministic transition $C\to D$, $C$ halts if and only if $D$ halts. Thus reverse use of defining equalities cannot create a false halting certificate. Boundary and erasure rules require explicit checking for every chosen encoding.

## ↑ Ancestors (10)

1. [Finite semigroup presentation](finite-semigroup-presentation.md)
2. [Semigroup presentation](semigroup-presentation.md)
3. [Semigroup](semigroup.md)
4. [Associative operation](associative-operation.md)
5. [Binary operation](binary-operation.md)
6. [Algebraic operation](algebraic-operation.md)
7. [Algebra](algebra-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-1/3/solution.md)
