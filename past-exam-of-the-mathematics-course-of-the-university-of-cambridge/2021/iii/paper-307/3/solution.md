<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Put $\theta=\theta^+$, $\bar\theta=\bar\theta^+$ and $y^+=x^++i\theta\bar\theta$. The general [two-dimensional N=(0,2) supersymmetry](../../../../../two-dimensional-n-0-2-supersymmetry.md) chiral superfield is

$$
\boxed{\Phi(y^+,x^-,\theta)=\phi(y^+,x^-)+\sqrt2\theta\psi_+(y^+,x^-)}.
$$

In ordinary coordinates this is $\Phi=\phi+\sqrt2\theta\psi_++i\theta\bar\theta\partial_+\phi$. A supersymmetric kinetic action is

$$
\boxed{S_1=-\frac i2\int d^2x\,d\theta d\bar\theta\,
\bar\Phi\partial_-\Phi},
$$

whose component form, up to light-cone conventions and total derivatives, is

$$
S_1=\int d^2x\left[-\partial_\mu\bar\phi\partial^\mu\phi
+i\bar\psi_+\partial_-\psi_+\right].
$$

A [Fermi superfield](../../../../../fermi-superfield.md) satisfying $\bar D_+\Lambda_-=f(\Phi)$ has expansion

$$
\boxed{\Lambda_-=\lambda_- -\sqrt2\theta G-\bar\theta f(\phi)
+\theta\bar\theta\left(i\partial_+\lambda_-
+\sqrt2\psi_+^i\partial_i f\right)}.
$$

Here $G$ is a complex bosonic [auxiliary field](../../../../../auxiliary-field.md). With the normalization in the question, the component action is

$$
\begin{aligned}
S_2=\int d^2x\bigg[&i\bar\lambda_-\partial_+\lambda_-+|G|^2
-\frac12|f|^2\\
&-\frac1{\sqrt2}\left(\bar\lambda_-\psi_+^i\partial_i f
+\bar\psi_+^{\bar i}\partial_{\bar i}\bar f\,\lambda_-\right)
\bigg],
\end{aligned}
$$

up to equivalent sign conventions for the fermions.

The chiral integral in $S_3$ is supersymmetric only if its integrand is chiral. Applying $\bar D_+$ gives the necessary and sufficient condition

$$
\boxed{\sum_a f_a(\Phi)J^a(\Phi)=0},
$$

with every $J^a$ holomorphic and with gauge charges chosen so that each product $\Lambda_{-a}J^a$ is gauge invariant. Its component expansion couples $G_a$ linearly to $J^a$ and supplies the corresponding Yukawa term $\lambda_{-a}\psi_+^i\partial_iJ^a$.

Eliminating each $G_a$ by its algebraic field equation gives the nonnegative scalar potential. In the normalization displayed above and in the question,

$$
\boxed{V(\phi)=\frac12\sum_a|f_a(\phi)|^2
+2\sum_a|J^a(\phi)|^2}.
$$

If the conventional definitions $\bar D_+\Lambda_-^a=\sqrt2E_a$ and $S_J=-\int d\theta\,\Lambda_{-a}J^a/\sqrt2+\mathrm{h.c.}$ are used instead, the same result is written $V=\sum_a(|E_a|^2+|J^a|^2)$; the two forms differ only by the normalization of $f$ and $J$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 307](../../paper-307-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
