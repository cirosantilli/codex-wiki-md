<h1 id="a/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [weak formulation](../../../../weak-formulation.md) is

$$
\boxed{\int_\Omega[Du\cdot D\phi+(u^3-u^2)\phi]dx=-\int_\Omega f\phi\,dx\quad(\phi\in H_0^1(\Omega)).}
$$

The boundary condition is encoded by $u\in H_0^1$. The [Sobolev embedding](../../../../failure-of-first-order-sobolev-embedding-into-linfinity-in-two-dimensions.md) in dimension three gives $H_0^1\hookrightarrow L^6$, hence also $L^4,L^3,L^2$ on the bounded domain. All energy terms and all the displayed pairings are therefore finite.

Pointwise, $t^4/4-t^3/3\geq t^4/8-C$ for a constant $C$, since the difference is a quartic with positive leading coefficient. The [Poincaré inequality](../../../../poincare-inequality.md) and [Young inequality](../../../../young-s-inequality-for-products.md) give $\int fv\geq-\tfrac14\|Dv\|_2^2-C_f$. Consequently

$$
I(v)\geq\frac14\|Dv\|_2^2+\frac18\|v\|_4^4-C_0.
$$

Thus the [infimum](../../../../infimum.md) is finite and a [minimizing sequence](../../../../minimizing-sequence.md) is bounded in $H_0^1$. Extract a weakly convergent subsequence there. The [Rellich-Kondrachov theorem](../../../../rellich-kondrachov-theorem.md) states that on a bounded $C^1$ domain in dimension three the embedding $H^1\hookrightarrow L^q$ is compact for $q<6$. A subsequence therefore converges strongly in $L^2,L^3,L^4$ to the same limit $u$. The potential terms and forcing converge, while the gradient [norm](../../../../norm.md) is weakly lower semicontinuous. The weak limit retains zero trace. Hence $I(u)\leq\liminf I(v_j)$ and **$u$ attains the absolute minimum**.

For any $\phi\in H_0^1$, the function $t\mapsto I(u+t\phi)$ has a minimum at zero. Differentiating its polynomial terms gives $\int[Du\cdot D\phi+(u^3-u^2+f)\phi]=0$. These differentiations are justified by the Sobolev integrability already noted. This is the [weak formulation](../../../../weak-formulation.md), proving **every energy minimizer is a [weak solution](../../../../weak-solution.md)**.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [A](../../a.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../split.md)
5. [Partial differential equations for pure and applied mathematicians and calculus of variations course of the University of Oxford](../../../../partial-differential-equations-for-pure-and-applied-mathematicians-and-calculus-of-variations-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
