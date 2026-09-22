<h1 id="30a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $u\in H_0^1(\Omega)$, both $u$ and its weak gradient are square integrable. The assumed bounds give $|F(u,x)|\le K(1+|u|^2)$, so the potential term is integrable and $E(u)$ is finite. Also

$$
E(u)\ge\tfrac12\|\nabla u\|_2^2-K|\Omega|,
$$

which is bounded below and coercive in $H_0^1$ by the [Poincaré inequality](../../../../../../poincare-inequality.md).

For distinct $u,v$ and $0<t<1$, convexity of $F$ and expansion of the squared gradient give

$$
E(tu+(1-t)v)\le tE(u)+(1-t)E(v)-\tfrac12t(1-t)\|\nabla(u-v)\|_2^2.
$$

The last norm is nonzero: a zero weak gradient makes $u-v$ constant, and its zero [trace](../../../../../../matrix-trace.md) forces that constant to vanish. Thus **$E$ is strictly convex**.

[Weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md) means that $u_j\rightharpoonup u$ in $H_0^1$ implies $E(u)\le\liminf_jE(u_j)$. A minimizing sequence is bounded by coercivity. Reflexivity of this Hilbert space gives a weakly convergent subsequence with limit still in $H_0^1$. The assumed [weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md) makes that limit a minimizer, and strict convexity makes it unique. Hence **$\boxed{E\text{ has exactly one minimizer in }H_0^1(\Omega)}$**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [30A](../../30a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2011](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
