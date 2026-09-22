<h1 id="3/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

**Yes: the procedure always terminates after finitely many steps.** If an iteration does not return, then $X_{i+1}\subsetneq X_i$. Thus at least one [state](../../../../../state-computer-science.md) is permanently removed. A finite [set](../../../../../set-split.md) of $|S|$ [states](../../../../../state-computer-science.md) can suffer at most $|S|$ such strict decreases, after which the next equality test must return. Therefore the procedure makes at most

$$
\boxed{|S|+1\text{ evaluations of }H}
$$

when started from $X_0=S$, counting the final evaluation that detects equality. The bound also covers $S=\varnothing$, where the first evaluation already returns. Each evaluation inspects finitely many [states](../../../../../state-computer-science.md) and successors, so every individual step terminates as well. Finiteness, rather than monotonicity alone, supplies this finite termination bound.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [3](../../3.md)
3. [Computer aided formal verification](../../../computer-aided-formal-verification-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
