<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Initial equilibrium at $a_I$ gives

$$
\langle p_{\mathbf q,i}(t_1)p_{-\mathbf q,j}(t_1)\rangle
=\delta_{ij}\frac{k_BT}{a_I+\kappa q^2}.
$$

The initial field and later noise are independent, so their cross terms vanish. Define

$$
\Delta t=t_2-t_1.
$$

With the supplied [Gaussian white noise](../../../../../../gaussian-white-noise.md) covariance, the noise contribution is

$$
2k_BT\Gamma\delta_{ij}
\int_{t_1}^{t_2}ds\,e^{-2r(q)(t_2-s)}
=\delta_{ij}\frac{k_BT}{a_F+\kappa q^2}
\left(1-e^{-2r(q)\Delta t}\right),
$$

Using the decay rate found in part (c), it follows that

$$
\langle p_{\mathbf q,i}(t_2)p_{-\mathbf q,j}(t_2)\rangle
=\delta_{ij}\left[
\frac{k_BT}{a_I+\kappa q^2}e^{-2r(q)\Delta t}
+\frac{k_BT}{a_F+\kappa q^2}
\left(1-e^{-2r(q)\Delta t}\right)
\right].
$$

This is the covariance interpolation in a [Gaussian Model A quench](../../../../../../gaussian-model-a-quench.md): each mode forgets its initial equilibrium with relaxation time $1/r(q)$ and approaches the final equilibrium variance. Larger-$q$ modes relax faster.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 344](../../../paper-344-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
