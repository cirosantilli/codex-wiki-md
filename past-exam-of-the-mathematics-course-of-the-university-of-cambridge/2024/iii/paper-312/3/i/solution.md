<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\theta=\nabla\mathbin\cdot\mathbf v$. Vanishing [vorticity](../../../../../../vorticity.md) implies in Fourier space

$$
\mathbf v(\mathbf q)=-i\frac{\mathbf q}{q^2}\theta(\mathbf q).
$$

Fourier transforming $\nabla\cdot(\delta\mathbf v)$ in the continuity equation gives

$$
\delta'(\mathbf k)+\theta(\mathbf k)
=-\int_{\mathbf q_1,\mathbf q_2}
\delta_D(\mathbf k-\mathbf q_1-\mathbf q_2)
\alpha(\mathbf q_1,\mathbf q_2)
\theta(\mathbf q_1)\delta(\mathbf q_2),
$$

with the [alpha mode-coupling kernel](../../../../../../alpha-mode-coupling-kernel.md)

$$
\boxed{\alpha(\mathbf q_1,\mathbf q_2)
=\frac{(\mathbf q_1+\mathbf q_2)\cdot\mathbf q_1}{q_1^2}}.
$$

Taking the divergence of $(\mathbf v\cdot\nabla)\mathbf v$ and symmetrizing its two velocity arguments gives

$$
\theta'(\mathbf k)+\mathcal H\theta(\mathbf k)
+\frac32\mathcal H^2\Omega_m\delta(\mathbf k)
=-\int_{\mathbf q_1,\mathbf q_2}
\delta_D(\mathbf k-\mathbf q_1-\mathbf q_2)
\beta(\mathbf q_1,\mathbf q_2)
\theta(\mathbf q_1)\theta(\mathbf q_2),
$$

where the [beta mode-coupling kernel](../../../../../../beta-mode-coupling-kernel.md) is

$$
\boxed{\beta(\mathbf q_1,\mathbf q_2)
=\frac{|\mathbf q_1+\mathbf q_2|^2
(\mathbf q_1\cdot\mathbf q_2)}{2q_1^2q_2^2}}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
