<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The same invariant interval can be written as $g_{\mu\nu}dx^\mu dx^\nu=\widetilde g_{\alpha\beta}d\widetilde x^\alpha d\widetilde x^\beta$. Applying the [chain rule](../../../../../../chain-rule.md) to the differentials proves the **metric transformation law**

$$
\boxed{g_{\mu\nu}(x)=
\frac{\partial\widetilde x^\alpha}{\partial x^\mu}
\frac{\partial\widetilde x^\beta}{\partial x^\nu}
\widetilde g_{\alpha\beta}(\widetilde x).}
$$

For first-order [scalar cosmological perturbations](../../../../../../scalar-cosmological-perturbation.md) and $\xi^\mu=(T,\partial^iL)$, compare perturbations at the same background coordinate label. Expanding the Jacobians and the shifted background gives the [linear metric gauge-transformation law](../../../../../../linear-metric-gauge-transformation-law.md)

$$
\widetilde{\delta g}_{\mu\nu}
=\delta g_{\mu\nu}-\mathcal L_\xi\bar g_{\mu\nu}.
$$

For the background $\bar g_{00}=-a^2$, $\bar g_{ij}=a^2\delta_{ij}$, the [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md) components are

$$
(\mathcal L_\xi\bar g)_{00}=-2a^2(T'+\mathcal HT),\qquad
(\mathcal L_\xi\bar g)_{0i}=a^2\partial_i(L'-T),
$$



$$
(\mathcal L_\xi\bar g)_{ij}=2a^2\mathcal HT\delta_{ij}
+2a^2\partial_i\partial_jL,
\qquad \mathcal H=\frac{a'}a.
$$

Here primes denote [conformal time](../../../../../../conformal-time.md) and $\mathcal H$ is the [conformal Hubble parameter](../../../../../../conformal-hubble-parameter.md). These expressions establish all four alternatives, including any chosen pair.

The $00$ component is $\delta g_{00}=-2a^2A$, immediately giving the [lapse function](../../../../../../lapse-function.md) perturbation transformation. The $0i$ component is $a^2\partial_iB$, giving the [shift vector](../../../../../../shift-vector.md) scalar-potential transformation. The trace of the spatial perturbation is $6a^2C$, so tracing the spatial [Lie derivative](../../../../../../lie-derivative-of-a-differential-form.md) gives the transformation of $C$. Its trace-free scalar part is $2a^2(\partial_i\partial_j-\delta_{ij}\nabla^2/3)E$, giving the transformation of $E$. Thus

$$
\boxed{\begin{aligned}
\widetilde A&=A-T'-\mathcal HT,\\
\widetilde B&=B+T-L',\\
\widetilde C&=C-\mathcal HT-\frac13\nabla^2L,\\
\widetilde E&=E-L.
\end{aligned}}
$$

As usual, identifying scalar potentials from their derivatives uses the standard boundary conditions, or nonzero Fourier modes, to remove homogeneous ambiguities.

At first order, [tensor cosmological perturbations](../../../../../../tensor-cosmological-perturbation.md) are spatial [transverse-traceless tensors](../../../../../../transverse-traceless-tensor.md). The coordinate-generated spatial perturbation consists of a trace term and symmetrized derivatives of the displacement. In [Fourier space](../../../../../../fourier-space.md), the latter terms carry a factor $k_i$ or $k_j$. The [transverse-traceless projector](../../../../../../transverse-traceless-projector.md) removes these longitudinal terms and the trace, including the derivative of a transverse vector displacement. Therefore **the tensor perturbation is gauge invariant at linear order around the homogeneous background**. This is a first-order statement, not a claim of automatic invariance at arbitrary perturbative order.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 310](../../../paper-310-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
