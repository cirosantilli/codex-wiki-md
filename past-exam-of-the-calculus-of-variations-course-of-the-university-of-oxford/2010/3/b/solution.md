<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the [direct method in the calculus of variations](../../../../direct-method-in-the-calculus-of-variations.md). The affine function $1-x$ is admissible with finite energy, and the energy is nonnegative since $2010$ is even. Thus $m=\inf I$ is finite. Choose a [minimizing sequence](../../../../minimizing-sequence.md) $u_n$ with uniformly bounded energy. Then

$$
\frac12\int_0^1|u_n'|^2dx\leq I(u_n)\leq C.
$$

The fixed value $u_n(0)=1$ and the [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) give $\|u_n\|_\infty\leq1+\|u_n'\|_2$ and $|u_n(x)-u_n(y)|\leq\|u_n'\|_2|x-y|^{1/2}$. Hence the sequence is bounded in $W^{1,2}$ and uniformly bounded and equicontinuous.

By [reflexivity](../../../../reflexive-relation.md) and the [Arzelà-Ascoli theorem](../../../../arzela-ascoli-theorem.md), pass to a subsequence with $u_n\rightharpoonup u$ in $W^{1,2}$ and $u_n\to u$ uniformly. The two limits coincide; [uniform convergence](../../../../uniform-convergence.md) also preserves $u(0)=1$, $u(1)=0$. Since all functions stay in a common bounded interval, [uniform convergence](../../../../uniform-convergence.md) gives $u_n^{2010}\to u^{2010}$ uniformly, and therefore convergence of the potential integrals. The [derivative](../../../../derivative.md) term is lower semicontinuous for [weak convergence](../../../../weak-convergence.md), so

$$
I(u)\leq\liminf_n\frac12\int|u_n'|^2+\lim_n\int u_n^{2010}=\liminf_nI(u_n)=m.
$$

Admissibility gives $I(u)\geq m$. Thus

$$
\boxed{I(u)=m,\quad\text{so the global minimum is attained}.}
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the calculus of variations course of the University of Oxford](../../../split.md)
5. [Calculus of variations course of the University of Oxford](../../../../calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
