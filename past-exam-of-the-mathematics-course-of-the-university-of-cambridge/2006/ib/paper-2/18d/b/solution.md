<h1 id="18d/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $W=\int_{-1}^1w(x)dx$, finite and positive. Exactness on the constant [polynomial](../../../../../../polynomial-split.md) gives $\sum_i a_i^{(n)}=W$. Positivity therefore implies the uniform operator bound $|I_n(h)|\leq W\|h\|_\infty$, and the [integral](../../../../../../integral.md) has the same bound.

For a continuous $f$ and $\epsilon>0$, the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md) gives a fixed [polynomial](../../../../../../polynomial-split.md) $Q$ of degree $m$ with $\|f-Q\|_\infty<\epsilon$. For every $n\geq m$, [polynomial](../../../../../../polynomial-split.md) exactness gives $I_n(Q)=I(Q)$. Thus

$$
\begin{aligned}
|I(f)-I_n(f)|&\leq |I(f-Q)|+|I_n(f-Q)|\\&\leq2W\|f-Q\|_\infty<2W\epsilon.
\end{aligned}
$$

Since $\epsilon$ is arbitrary, $\boxed{I_n(f)\to I(f)}$ for every continuous $f$. This is [convergence of positive quadrature on continuous functions](../../../../../../convergence-of-positive-quadrature-on-continuous-functions.md). The argument requires nodes in $[-1,1]$, implicit in a rule defined on all continuous functions there; otherwise their function values would not even be specified by the stated domain. Exactness alone would not provide the norm bound if arbitrarily signed weights were allowed.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [18D](../../18d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
