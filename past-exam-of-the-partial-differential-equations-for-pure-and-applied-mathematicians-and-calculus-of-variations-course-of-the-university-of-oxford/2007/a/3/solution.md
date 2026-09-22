<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Bounded coefficients and Cauchy-Schwarz give $|B[u,v]|\leq C\|u\|_{H^1}\|v\|_{H^1}$. [Uniform ellipticity](../../../../uniformly-elliptic-operator.md) gives $B[u,u]\geq\theta\|Du\|_2^2$ because $c\geq0$. [Poincaré inequality](../../../../poincare-inequality.md) $\|u\|_2\leq C_P\|Du\|_2$ holds on $H_0^1$ of a bounded domain, so

$$
\boxed{B[u,u]\geq\nu\|u\|_{H^1}^2,\qquad\nu=\theta/(1+C_P^2)>0.}
$$

A [weak solution](../../../../weak-solution.md) is $u\in H_0^1$ satisfying $B[u,\phi]=\int f\phi$ for every $\phi\in H_0^1$. The energy is finite by boundedness of $B$ and the forcing functional, and

$$
I(v)\geq\frac\nu2\|v\|_{H^1}^2-\|f\|_2\|v\|_{H^1}\geq\frac\nu4\|v\|_{H^1}^2-C_f.
$$

It is bounded below and a [minimizing sequence](../../../../minimizing-sequence.md) is bounded in the [Hilbert space](../../../../hilbert-space-split.md) $H_0^1$. Its [closed linear span](../../../../closed-linear-span.md) is [separable](../../../../separable-topological-space.md), so part 1 supplies a [weakly convergent](../../../../weak-convergence.md) [subsequence](../../../../subsequence.md) with limit $u$. Symmetry and nonnegativity of $B$ show

$$
B[v_j,v_j]=B[u,u]+2B[u,v_j-u]+B[v_j-u,v_j-u]\geq B[u,u]+o(1).
$$

The forcing term converges by [weak convergence](../../../../weak-convergence.md). Thus $I(u)\leq\liminf I(v_j)$, proving attainment. [First variation](../../../../first-variation.md) in every zero-trace direction gives the weak equation. If $u,w$ are two solutions, test their difference equation with $u-w$ and use coercivity to get $u=w$. Hence **there is exactly one [weak solution](../../../../weak-solution.md), and it is the unique energy minimizer**. Indeed $I(v)-I(u)=\tfrac12B[v-u,v-u]$ directly verifies the minimizing property.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
