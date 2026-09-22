# Two-vertex branching comparison for contact-process survival

↑ **Parent:** [Global survival threshold of the contact process](global-survival-threshold-of-the-contact-process.md)

Inside a rooted $d$-ary subtree of a degree-$(d+1)$ [regular tree](regular-tree.md), pair each cell root with one distinguished child. Keep reinfection inside each pair, suppress infection back into its parent cell, and allow each child cell to be activated only once. Offspring counts of different cells are independent and identically distributed, so cell genealogies form a [Galton-Watson process](galton-watson-process.md). A cell root has $d-1$ outgoing child-cell [edges](edge-of-a-graph.md) and its paired [vertex](vertex-graph-theory.md) has $d$. Starting at the root, the [probabilities](probability.md) to send an arrow along one specified outgoing [edge](edge-of-a-graph.md) from these two [vertices](vertex-graph-theory.md) before internal extinction are respectively

$$
a=\frac{2\lambda^3+3\lambda^2+2\lambda}{D},\qquad b=\frac{2\lambda^3+2\lambda^2}{D},\qquad D=2\lambda^3+4\lambda^2+5\lambda+2.
$$

They follow by first-step equations on the three nonempty pair states. The offspring mean is $M=(d-1)a+db$, and

$$
M\bigl(1/(d-1)\bigr)-1=\frac{2(d-1)}{2d^3-d^2+1}>0.
$$

Continuity makes $M>1$ at some strictly smaller positive rate. The [branching-process extinction criterion](branching-process-extinction-criterion.md) then gives positive survival [probability](probability.md) for the suppressed process, hence for the original [contact process](contact-process.md).

## ↑ Ancestors (10)

1. [Global survival threshold of the contact process](global-survival-threshold-of-the-contact-process.md)
2. [Survival probability of the contact process](survival-probability-of-the-contact-process.md)
3. [Contact process](contact-process.md)
4. [Interacting particle system](interacting-particle-system.md)
5. [Stochastic process](stochastic-process-split.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-28/2/solution.md)
