<h1 id="10/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A [Turing machine](../../../../../turing-machine.md) has a finite control, an unbounded tape divided into cells over a finite tape [alphabet](../../../../../alphabet.md) including a blank symbol, and a head that reads one cell at a time. For a deterministic [Turing machine](../../../../../turing-machine.md), the current state and scanned symbol determine the replacement symbol, a head move one cell left or right, and the next state. The input occupies finitely many cells initially; all other cells are blank. Distinguished halting states report acceptance or rejection.

A [formal language](../../../../../formal-language.md) is a [decidable language](../../../../../recursive-language.md) if some [Turing machine](../../../../../turing-machine.md) halts on every input [string](../../../../../string.md), accepting exactly the members and rejecting all nonmembers:

$$
\boxed{L\text{ is decidable}\iff\exists M\ \forall w,\ M(w)\text{ halts and accepts exactly when }w\in L.}
$$

Halting on the nonmembers is part of the requirement; a machine that merely runs forever on some nonmembers need not decide the [formal language](../../../../../formal-language.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [10](../../10.md)
3. [Calculus, linear algebra, discrete mathematics, logic and proof, and models of computation](../../../calculus-linear-algebra-discrete-mathematics-logic-and-proof-and-models-of-computation-split.md)
4. [2005](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
