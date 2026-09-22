<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

First prove the hinted [Caccioppoli inequality](../../../../../../caccioppoli-inequality.md). Testing the [weak formulation](../../../../../../weak-formulation.md) with $u_k\varphi^2$ is legitimate by approximation in the zero-boundary [Sobolev space](../../../../../../sobolev-space-split.md). Let $\Lambda_*=\operatorname*{ess\,sup}\|a(x)\|_{\mathrm{op}}\leq n\Lambda$. Then

$$
\lambda\int|Du_k|^2\varphi^2
\leq2\Lambda_*\int|u_k|\,|Du_k|\,|\varphi|\,|D\varphi|
\leq\tfrac\lambda2\int|Du_k|^2\varphi^2
+\frac{2\Lambda_*^2}{\lambda}\int u_k^2|D\varphi|^2,
$$

by [Young inequality](../../../../../../young-s-inequality-for-products.md). Hence

$$
\boxed{\int|Du_k|^2\varphi^2\leq\frac{4\Lambda_*^2}{\lambda^2}\int u_k^2|D\varphi|^2.}
$$

No derivative of the measurable coefficient [matrix](../../../../../../matrix.md) is taken.

Set $w_k=u_k/\sup_{B_1}|u_k|$. The denominator is finite and positive because $u_k$ is continuous on the compact closure and nonzero. Each $w_k$ solves the same linear equation and $|w_k|\leq1$. For every $\theta<1$, choose a [cutoff function](../../../../../../cutoff-function.md) equal to one on $B_\theta$ and supported in a slightly larger interior [Euclidean ball](../../../../../../euclidean-ball.md). The energy bound gives a uniform $W^{1,2}(B_\theta)$ bound.

Take radii $\theta_j\uparrow1$. Weak compactness and a [diagonal subsequence argument](../../../../../../diagonal-subsequence-argument.md) produce one subsequence converging weakly in $W^{1,2}(B_{\theta_j})$ for every $j$, with consistent restrictions defining $v\in W^{1,2}_{\mathrm{loc}}(B_1)$. Part (b) and the [Arzelà-Ascoli theorem](../../../../../../arzela-ascoli-theorem.md) allow a further subsequence converging uniformly on $\overline{B_{1/4}}$. Its uniform limit agrees almost everywhere with the weak limit and supplies its continuous representative there.

For every smooth compactly supported [test function](../../../../../../test-function.md), choose $j$ containing its support. Since $a^{ij}D_i\varphi\in L^2$ and $Dw_k$ converges weakly there,

$$
\int a^{ij}D_jvD_i\varphi
=\lim_k\int a^{ij}D_jw_kD_i\varphi=0.
$$

Thus the [compactness of normalized weak elliptic solutions](../../../../../../compactness-of-normalized-weak-elliptic-solutions.md) gives

$$
\boxed{w_{k'}\longrightarrow v\text{ uniformly on }\overline{B_{1/4}},\qquad
Lv=0\text{ weakly in every }B_\theta,\ 0<\theta<1.}
$$

The diagonal step is needed to retain the equation beyond the small [Euclidean ball](../../../../../../euclidean-ball.md) of [uniform convergence](../../../../../../uniform-convergence.md). The limit need not be nonzero: for the [Laplacian](../../../../../../laplacian.md) in dimension at least two, the normalized [harmonic functions](../../../../../../harmonic-function.md) $\operatorname{Re}(x_1+ix_2)^k$ tend uniformly to zero on each smaller [Euclidean ball](../../../../../../euclidean-ball.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
