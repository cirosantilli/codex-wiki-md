<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The required functional, with the sign appropriate to a positive divergence operator, is

$$
\boxed{\mathcal F(u)=\frac12Q(u,u)+\int_\Omega fu\,dx.}
$$

It is differentiable on $W_0^{1,2}$, with $D\mathcal F(u)[v]=Q(u,v)+\int fv$. A critical point consequently satisfies the weak equation. We now prove existence by the [direct method in the calculus of variations](../../../../../../direct-method-in-the-calculus-of-variations.md), rather than invoke the representation theorem again.

The ellipticity and Poincare estimates imply

$$
\mathcal F(u)\geq\frac\lambda2\|Du\|_2^2-C_P\|f\|_2\|Du\|_2
\geq\frac\lambda4\|Du\|_2^2-\frac{C_P^2}\lambda\|f\|_2^2.
$$

Thus the infimum is finite and any [minimizing sequence](../../../../../../minimizing-sequence.md) is bounded in the [Sobolev norm](../../../../../../sobolev-norm.md). A bounded sequence in a [Hilbert space](../../../../../../hilbert-space-split.md) has a [weakly convergent](../../../../../../weak-convergence.md) subsequence; write $u_j\rightharpoonup u$ in $W_0^{1,2}$. The equivalent $Q$ norm has the same continuous linear functionals and hence the same [weak convergence](../../../../../../weak-convergence.md). A Hilbert norm is [Weak lower semicontinuity](../../../../../../weak-lower-semicontinuity.md), giving $Q(u,u)\leq\liminf_jQ(u_j,u_j)$. The term $\int fu_j$ converges to $\int fu$ because it is a [bounded linear functional](../../../../../../continuous-linear-functional.md). Therefore

$$
\mathcal F(u)\leq\liminf_j\mathcal F(u_j)=\inf\mathcal F.
$$

The limit attains the infimum. Differentiating $t\mapsto\mathcal F(u+tv)$ at its minimum, for every $v$, gives $D\mathcal F(u)[v]=0$. This produces the desired [weak solution](../../../../../../weak-solution.md). Strict positivity of $Q$ also makes the functional [strictly convex](../../../../../../strictly-convex-function.md), consistent with uniqueness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
