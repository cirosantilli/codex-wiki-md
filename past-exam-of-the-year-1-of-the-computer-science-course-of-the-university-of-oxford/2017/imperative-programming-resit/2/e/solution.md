<h1 id="2/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Maintain that all positive $h<\mathrm{lo}$ fail $rh^2\geq i^2$, while `hi` satisfies that inequality; its least satisfying integer lies in $[\mathrm{lo},\mathrm{hi}]$. Monotonicity of $rk^2$ in positive $k$ validates both updates. At exit the endpoints agree and identify exactly that least integer.

The [loop variant](../../../../../loop-variant.md) `hi-lo` decreases on every iteration and is at least halved up to rounding. Starting with at most $i$ candidates therefore needs **$O(\log(i+1))$ arithmetic operations**, conventionally $O(\log i)$ for $i\geq2$. For $i=1$ the loop is empty. The final upper-bound check proves the returned Boolean is the required membership answer.

## ↑ Ancestors (12)

1. [E](../e.md)
2. [2](../../2.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
