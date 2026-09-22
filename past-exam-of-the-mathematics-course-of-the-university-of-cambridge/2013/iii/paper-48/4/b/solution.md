<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Promote the canonical field and momentum $\pi=f'$ to operators satisfying the [canonical commutation relation](../../../../../../canonical-commutation-relation.md), $[\hat f(\tau,\mathbf x),\hat\pi(\tau,\mathbf y)]=i\delta^{(3)}(\mathbf x-\mathbf y)$. A real field has Fourier reality condition $\hat f_{\mathbf k}^\dagger=\hat f_{-\mathbf k}$. Its oscillator expansion is

$$
\boxed{\hat f_{\mathbf k}=u_k\hat a_{\mathbf k}+u_k^*\hat a_{-\mathbf k}^\dagger}.
$$

The [creation and annihilation operators](../../../../../../creation-and-annihilation-operators.md) add or remove excitations in the selected mode basis, with

$$
[\hat a_{\mathbf k},\hat a_{\mathbf k'}^\dagger]=\delta^{(3)}(\mathbf k-\mathbf k'),\qquad
[\hat a_{\mathbf k},\hat a_{\mathbf k'}]=[\hat a_{\mathbf k}^\dagger,\hat a_{\mathbf k'}^\dagger]=0,\qquad
\hat a_{\mathbf k}|0\rangle=0.
$$

Canonical normalization requires the [Wronskian](../../../../../../wronskian.md) $u_ku_k^{*\prime}-u_k^*u_k'=i$.

For the [Bunch-Davies vacuum](../../../../../../bunch-davies-vacuum.md), choose the positive-frequency short-wavelength behavior $u_k\sim e^{-ik\tau}/\sqrt{2k}$ as $k|\tau|\to\infty$. For the proposed solution, direct differentiation gives

$$
u_k'=\frac{e^{-ik\tau}}{\sqrt{2k}}\left[-ik-\frac1\tau+\frac{i}{k\tau^2}\right],\qquad
u_k''=\frac{e^{-ik\tau}}{\sqrt{2k}}\left[-k^2+\frac{ik}\tau+\frac2{\tau^2}-\frac{2i}{k\tau^3}\right].
$$

Substitution cancels every term in $u_k''+(k^2-2/\tau^2)u_k$. Its [Wronskian](../../../../../../wronskian.md) is $i$, and its large-$|k\tau|$ limit is the required flat-spacetime positive-frequency mode. Thus

$$
\boxed{u_k=\frac{e^{-ik\tau}}{\sqrt{2k}}\left(1-\frac{i}{k\tau}\right)}.
$$

A term with the conjugate frequency is another allowed classical solution, but would describe a different quantum state, through a [Bogoliubov transformation](../../../../../../bogoliubov-transformation.md). Its coefficient is set to zero by the early-time vacuum condition, not by absence of a second solution to the differential equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
