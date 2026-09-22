<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the Fourier convention $f(\mathbf x)=\int_{\mathbf k}f(\mathbf k)e^{i\mathbf k\cdot\mathbf x}$ with $\int_{\mathbf k}=\int d^3k/(2\pi)^3$. Neglect [anisotropic stress](../../../../../../scalar-anisotropic-stress.md) and assume the pressureless velocity is irrotational, so

$$
\mathbf v(\mathbf k)=-i\frac{\mathbf k}{k^2}\theta(\mathbf k).
$$

Fourier transforming $\nabla\mathbin\cdot(\delta\mathbf v)$ in the nonlinear continuity equation gives

$$
\delta'(\mathbf k)+\theta(\mathbf k)
=-\int_{\mathbf k_1\mathbf k_2}
(2\pi)^3\delta_D(\mathbf k_1+\mathbf k_2-\mathbf k)
\alpha(\mathbf k_1,\mathbf k_2)
\theta(\mathbf k_1)\delta(\mathbf k_2),
$$

where the [alpha mode-coupling kernel](../../../../../../alpha-mode-coupling-kernel.md) and its symmetrization are

$$
\alpha(\mathbf k_1,\mathbf k_2)
=\frac{(\mathbf k_1+\mathbf k_2)\cdot\mathbf k_1}{k_1^2},
$$



$$
\boxed{\alpha_s
=1+\frac{\mathbf k_1\cdot\mathbf k_2}{2}
\left(\frac1{k_1^2}+\frac1{k_2^2}\right)}.
$$

Taking the divergence of the Euler equation gives

$$
\theta'+\mathcal H\theta+\frac32\mathcal H^2\delta
=-\int_{\mathbf k_1\mathbf k_2}
(2\pi)^3\delta_D(\mathbf k_1+\mathbf k_2-\mathbf k)
\beta(\mathbf k_1,\mathbf k_2)
\theta(\mathbf k_1)\theta(\mathbf k_2),
$$

with the symmetric [beta mode-coupling kernel](../../../../../../beta-mode-coupling-kernel.md)

$$
\boxed{\beta(\mathbf k_1,\mathbf k_2)
=\frac{|\mathbf k_1+\mathbf k_2|^2
(\mathbf k_1\cdot\mathbf k_2)}{2k_1^2k_2^2}}.
$$

In the [Einstein-de Sitter universe](../../../../../../einstein-de-sitter-universe.md), $a'=\mathcal Ha$ and $\mathcal H'=-\mathcal H^2/2$. At linear order the ansatz gives $\widetilde\theta^{(1)}=\widetilde\delta^{(1)}$. At second order, the continuity and Euler equations become

$$
2\widetilde\delta^{(2)}-\widetilde\theta^{(2)}
=\int\alpha_s\widetilde\delta^{(1)}\widetilde\delta^{(1)},
$$



$$
3\widetilde\delta^{(2)}-5\widetilde\theta^{(2)}
=-2\int\beta\widetilde\delta^{(1)}\widetilde\delta^{(1)},
$$

where each integral includes the momentum-conserving measure above. Eliminating $\widetilde\theta^{(2)}$ yields

$$
\widetilde\delta^{(2)}(\mathbf k)
=\int_{\mathbf k_1\mathbf k_2}(2\pi)^3\delta_D(\mathbf k_1+\mathbf k_2-\mathbf k)
F_2(\mathbf k_1,\mathbf k_2)
\widetilde\delta^{(1)}(\mathbf k_1)
\widetilde\delta^{(1)}(\mathbf k_2),
$$

with the [standard perturbation theory density kernel](../../../../../../standard-perturbation-theory-density-kernel.md)

$$
\boxed{F_2=\frac57\alpha_s+\frac27\beta}.
$$

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
