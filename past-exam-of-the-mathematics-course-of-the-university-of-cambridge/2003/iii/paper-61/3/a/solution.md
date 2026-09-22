<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Put $\theta=kx-4k^3t$. Conjugation by $e^{i\theta\sigma_3}$ is the meaning of $e^{i\theta\widehat\sigma_3}$. The normalized eigenfunctions have the [Volterra integral equation](../../../../../../volterra-integral-equation.md) representation

$$
\mu_j=I+\int_{\gamma_j}e^{i[k(x-x')-4k^3(t-t')]\widehat\sigma_3}
[Q\mu_j\,dx'+\widetilde Q\mu_j\,dt'].
$$

Choose $\gamma_1$ from $(0,T)$ down the time boundary and then right, $\gamma_2$ from $(0,0)$ up the time boundary and then right, and $\gamma_3$ horizontally from infinity. Compatibility of the [Lax pair](../../../../../../lax-pair.md) makes the resulting construction path-independent.

Let $a=\operatorname{Im}k$ and $b=\operatorname{Im}k^3$. The nontrivial exponential in column one has modulus $e^{2a(x-x')-8b(t-t')}$; column two has its reciprocal. For $\gamma_1$, $x-x'\ge0$ and $t-t'\le0$, giving signs $a,b\le0$ for column one and $a,b\ge0$ for column two. For $\gamma_2$, both differences are nonnegative, giving $(a\le0,b\ge0)$ and $(a\ge0,b\le0)$. For $\gamma_3$, $x-x'\le0$ and the time difference is zero, giving upper and lower half-planes, respectively.

Define $D_1:(a>0,b>0)$, $D_2:(a>0,b<0)$, $D_3:(a<0,b>0)$ and $D_4:(a<0,b<0)$. The bounded analytic column domains are therefore

$$
\boxed{\mu_1:(D_4,D_1),\qquad\mu_2:(D_3,D_2),\qquad
\mu_3:(\mathbb C_+,\mathbb C_-).}
$$

These are the [Volterra analyticity sectors for reverse-dispersion mKdV](../../../../../../volterra-analyticity-sectors-for-reverse-dispersion-mkdv.md), shown in the right panel of the figure. $D_1$ is the pair of upper outer sectors, $D_2$ the upper middle sector, $D_3$ the lower middle sector and $D_4$ the lower outer pair. Their boundaries are the six rays $\arg k=m\pi/3$. The [Volterra integral equation](../../../../../../volterra-integral-equation.md) converges and differentiates analytically where these kernels are bounded, assuming the usual sufficiently integrable spatial decay and smoothness needed by these normalizations. If decay is interpreted as merely pointwise convergence to zero without an integrability condition, existence and the stated large-$k$ normalization need additional hypotheses. A finite-path eigenfunction may be entire for fixed coordinates, but boundedness for large $k$ holds in the displayed domains; entire continuation does not enlarge those bounded sectors.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
