<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose coordinates $(q_1,\ldots,q_n,p_1,\ldots,p_n)$ with [standard symplectic form](../../../../../../standard-symplectic-form.md) $\omega_0=\sum_jdq_j\wedge dp_j$, and regard the given sphere $S$ as lying in $\{p_n=0\}$. With $\iota_{X_H}\omega_0=-dH$, the linear [Hamiltonian function](../../../../../../hamiltonian-function.md) $H_\delta=\delta q_n$ has [Hamiltonian vector field](../../../../../../hamiltonian-vector-field.md) $\delta\partial_{p_n}$ and translates in the missing coordinate.

To make this a permissible compactly supported map, take a smooth cutoff $\chi$ equal to one on an open neighbourhood of the fixed compact swept set

$$
\{z+s e_{p_n}:z\in S,\ |s|\leq1\}.
$$

Choose $\chi$ with compact support and let $R=\sup_{\operatorname{supp}\chi}|q_n|<\infty$. For $0<\delta<1$ put $G_\delta=\delta q_n\chi$. On the whole swept region the cutoff is locally constant, so its derivatives vanish and $X_{G_\delta}=\delta\partial_{p_n}$. Thus the flow carries every $z\in S$ to $z+t\delta e_{p_n}$ for $0\leq t\leq1$.

The time-one image lies in $\{p_n=\delta\}$ and is disjoint from the original sphere. Its [Hofer metric from the spatial supremum norm](../../../../../../hofer-metric-from-the-spatial-supremum-norm.md) obeys

$$
\rho_\infty(\mathrm{id},\phi_{G_\delta}^1)\leq\|G_\delta\|_\infty\leq R\delta.
$$

In the oscillation convention the upper bound is $2R\delta$. Since $\delta$ can approach zero while the cutoff and $R$ stay fixed,

$$
\boxed{e(S)=0}.
$$

This proves the [zero displacement energy for a compact set in a hyperplane](../../../../../../zero-displacement-energy-for-a-compact-set-in-a-hyperplane.md); it does not assert that any one nonidentity displacing map has zero norm.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
