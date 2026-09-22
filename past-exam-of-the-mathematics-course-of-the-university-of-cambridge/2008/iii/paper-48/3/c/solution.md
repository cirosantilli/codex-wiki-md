<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Denote the momentum in the printed mode expansion by $\widetilde\pi^\nu$, as it equals $-\dot A^\nu$ for the boundary-subtracted density discussed in part (b). Take a real complete basis of [polarization vectors](../../../../../../polarization-vector.md). Its completeness relation with one index raised is

$$
\sum_{\lambda,\lambda'}\epsilon_\mu^\lambda(\mathbf p)
\epsilon^{\nu\lambda'}(\mathbf p)\eta^{\lambda\lambda'}=\delta_\mu{}^\nu.
$$

Here raising or lowering the polarization labels uses the same diagonal matrix $\eta$, so this is just the completeness relation in the PDF. Write $\mathbf r=\mathbf x-\mathbf y$. In the mixed field-momentum [commutator](../../../../../../commutator.md), the $aa^\dagger$ term gives the product of the minus sign in $\widetilde\pi$'s creation part and the minus sign in the oscillator [commutator](../../../../../../commutator.md). The $a^\dagger a$ term gives the same sign. The two mode normalization factors multiply to $1/2$, and the momentum delta function removes one integral. Consequently

$$
\begin{aligned}
[A_\mu(\mathbf x),\widetilde\pi^\nu(\mathbf y)]
&=\frac i2\int\frac{d^3p}{(2\pi)^3}
\sum_{\lambda,\lambda'}\epsilon_\mu^\lambda\epsilon^{\nu\lambda'}\eta^{\lambda\lambda'}
\left(e^{i\mathbf p\cdot\mathbf r}+e^{-i\mathbf p\cdot\mathbf r}\right)\\
&=i\delta_\mu{}^\nu\delta^{(3)}(\mathbf x-\mathbf y).
\end{aligned}
$$

For the field-field [commutator](../../../../../../commutator.md), the polarization sum gives instead

$$
[A_\mu(\mathbf x),A_\nu(\mathbf y)]
=-\eta_{\mu\nu}\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r}-e^{-i\mathbf p\cdot\mathbf r}}{2|\mathbf p|}=0,
$$

because the integrand is odd under $\mathbf p\mapsto-\mathbf p$. Similarly,

$$
[\widetilde\pi^\mu(\mathbf x),\widetilde\pi^\nu(\mathbf y)]
=-\eta^{\mu\nu}\int\frac{d^3p}{(2\pi)^3}\frac{|\mathbf p|}{2}
\left(e^{i\mathbf p\cdot\mathbf r}-e^{-i\mathbf p\cdot\mathbf r}\right)=0.
$$

These are the requested [canonical commutation relations](../../../../../../canonical-commutation-relation.md), derived by [photon oscillator completeness and canonical brackets](../../../../../../photon-oscillator-completeness-and-canonical-brackets.md).

They also hold for the literal momenta of part (b). The shifts are

$$
\pi^0=\widetilde\pi^0+\partial_iA_i,\qquad
\pi^i=\widetilde\pi^i-\partial_iA_0.
$$

Since the fields commute at equal times, their mixed brackets with the momenta do not change. The only potentially new momentum bracket is

$$
[\pi^0(\mathbf x),\pi^i(\mathbf y)]
=i\bigl(\partial_{y^i}+\partial_{x^i}\bigr)\delta^{(3)}(\mathbf x-\mathbf y)=0.
$$

All other momentum brackets vanish separately. Thus **both canonical conventions have $[A_\mu,\pi^\nu]=i\delta_\mu{}^\nu\delta^3$ and vanishing coordinate-coordinate and momentum-momentum brackets**, even though the momentum operators differ by spatial derivatives. This resolves the density/expansion mismatch without changing the printed oscillator algebra.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 48](../../../paper-48-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
