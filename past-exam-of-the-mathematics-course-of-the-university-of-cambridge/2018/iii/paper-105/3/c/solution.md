<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Take $\psi\in L^2(U)$, the natural initial-data assumption needed for the requested $L^2$ convergence but not explicitly stated in this subpart. Use the genuine Dirichlet eigensystem from part (b)(iii) and put $\psi_m=(\psi,w_m)$. The [spectral construction of a parabolic solution](../../../../../../spectral-construction-of-a-parabolic-solution.md) is

$$
\boxed{u(t,x)=\sum_{m=1}^\infty e^{-\lambda_mt}\psi_mw_m(x).}
$$

Each finite sum has zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) and satisfies $u_t+Lu=0$.

To justify all derivatives, fix $\varepsilon>0$. For any integers $k,j\geq0$, the squared $X_k$ norm of a tail of the $j$th time derivative is

$$
\sum_{m>N}\lambda_m^{k+2j}e^{-2t\lambda_m}|\psi_m|^2
\leq\sup_{\lambda\geq\lambda_1}\bigl(\lambda^{k+2j}e^{-2\varepsilon\lambda}\bigr)
\sum_{m>N}|\psi_m|^2\longrightarrow0
$$

uniformly for $t\geq\varepsilon$. Use the corrected [Sobolev domains of powers of an elliptic Dirichlet operator](../../../../../../sobolev-domains-of-powers-of-an-elliptic-dirichlet-operator.md), not the inaccurate unqualified assertion in the PDF. Their norm equivalence gives convergence in every ordinary $H^k$. The [Sobolev embedding theorem](../../../../../../sobolev-embedding-theorem.md) then gives convergence of every desired spatial derivative by choosing $k$ large enough. Thus termwise differentiation is justified, $u\in C^\infty(U_T)$, and $u(t,\cdot)\in C^\infty(\overline U)$ for every $t>0$. The trace remains zero, and $u_t+Lu=0$ holds pointwise.

Finally [Parseval identity](../../../../../../parseval-identity.md) gives

$$
\|u(t)-\psi\|_2^2=\sum_m(1-e^{-t\lambda_m})^2|\psi_m|^2\longrightarrow0
$$

by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md), since each factor tends to zero and is bounded by one. No boundary compatibility of the initial $L^2$ data is required for positive-time smoothness.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
