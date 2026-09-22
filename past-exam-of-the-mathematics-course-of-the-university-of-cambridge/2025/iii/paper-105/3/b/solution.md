<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $u_0\in L^\infty(\mathbb R)$, call $u\in L^\infty(\mathbb R_+\times\mathbb R)$ a [weak solution](../../../../../../weak-solution.md) when, for every $\varphi\in C_c^1([0,\infty)\times\mathbb R)$,

$$
\int_0^\infty\!\int_{\mathbb R}
\left[u\bigl(\varphi_t+(F\varphi)_x\bigr)+g\varphi\right]dx\,dt
+\int_{\mathbb R}u_0(x)\varphi(0,x)\,dx=0.
$$

This follows by multiplying the equation by a [test function](../../../../../../test-function.md) and applying [integration by parts](../../../../../../integration-by-parts.md) in time and space; $(F\varphi)_x$ includes the term $F_x\varphi$ because the original transport operator is not in divergence form.

If $u$ is $C^1$, test functions supported away from $t=0$ show that $u_t+Fu_x=g$ as a [distributional identity](../../../../../../distributional-identity.md), hence pointwise. Integrating this pointwise equation by parts in the weak identity leaves

$$
\int_{\mathbb R}(u(0,x)-u_0(x))\varphi(0,x)\,dx=0.
$$

Arbitrary boundary test functions and the [fundamental lemma of the calculus of variations](../../../../../../fundamental-lemma-of-the-calculus-of-variations.md) give $u(0,x)=u_0(x)$. Thus a $C^1$ weak solution is the unique classical solution from part a.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
