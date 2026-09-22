<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The exact solution is feasible because

$$
\|Au^\dagger-f^\delta\|_Y=\|f-f^\delta\|_Y\leq\delta\leq c\delta.
$$

The feasible set $E_\delta$ is convex and weakly closed. A minimizing sequence has bounded residual and bounded $J$; the coercivity assumption from part (a), applied to a fixed positive weighted objective, makes it bounded in $X$. Reflexivity gives a weakly convergent subsequence, and weak lower semicontinuity of the residual and $J$ keeps its limit feasible and minimizing.

Since $\widehat u_\delta$ minimizes $J$ over $E_\delta$,

$$
J(\widehat u_\delta)\leq J(u^\dagger).
$$

The [source condition in variational regularization](../../../../../../source-condition-in-variational-regularization.md) and feasibility then yield

$$
\begin{aligned}
D_J^{p^\dagger}(\widehat u_\delta,u^\dagger)
&\leq-\langle w^\dagger,A\widehat u_\delta-f\rangle\\
&\leq\|w^\dagger\|_{Y^*}
\left(\|A\widehat u_\delta-f^\delta\|_Y
+\|f^\delta-f\|_Y\right)\\
&\leq(c+1)\|w^\dagger\|_{Y^*}\delta.
\end{aligned}
$$

Thus the claimed constant is $\boxed{C=(c+1)\|w^\dagger\|_{Y^*}}$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
