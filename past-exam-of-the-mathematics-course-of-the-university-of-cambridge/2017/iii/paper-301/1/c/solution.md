<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the supplied oscillator expansion, with the boundary-term convention for [momentum](../../../../../../momentum.md) stated in part (b). Use a real [polarization vector](../../../../../../polarization-vector.md) basis, as in the supplied unconjugated [polarization completeness relation](../../../../../../polarization-completeness-relation.md). Raise its second field index to obtain

$$
\sum_{\lambda,\lambda'}\epsilon_\mu^\lambda\epsilon^{\nu\lambda'}\eta^{\lambda\lambda'}=\delta_\mu{}^\nu.
$$

The mixed [commutator](../../../../../../commutator.md) contains only the annihilation-creation and creation-annihilation terms. Their signs are both positive after combining the minus sign in the [momentum](../../../../../../momentum.md) expansion with the negative [Minkowski metric](../../../../../../minkowski-metric.md) oscillator [commutator](../../../../../../commutator.md). Setting $\mathbf r=\mathbf x-\mathbf y$ and using the [momentum](../../../../../../momentum.md) [Dirac delta distribution](../../../../../../dirac-delta-function.md) gives

$$
[A_\mu(\mathbf x),\pi^\nu(\mathbf y)]
=\frac i2\delta_\mu{}^\nu\int\frac{d^3p}{(2\pi)^3}\bigl(e^{i\mathbf p\cdot\mathbf r}+e^{-i\mathbf p\cdot\mathbf r}\bigr)
=i\delta_\mu{}^\nu\delta^3(\mathbf r).
$$

Here the last equality is the [Fourier representation of the Dirac delta function](../../../../../../fourier-representation-of-the-dirac-delta-function.md). Similarly,

$$
[A_\mu(\mathbf x),A_\nu(\mathbf y)]
=-\eta_{\mu\nu}\int\frac{d^3p}{(2\pi)^3}\frac{e^{i\mathbf p\cdot\mathbf r}-e^{-i\mathbf p\cdot\mathbf r}}{2|\mathbf p|}=0,
$$

because the integrand is odd under $\mathbf p\mapsto-\mathbf p$. The momentum-momentum [commutator](../../../../../../commutator.md) is proportional to the same odd difference, now weighted by $|\mathbf p|/2$, and also vanishes. Therefore the equal-time [canonical commutation relations](../../../../../../canonical-commutation-relation.md) are

$$
\boxed{[A_\mu(\mathbf x),\pi^\nu(\mathbf y)]=i\delta_\mu{}^\nu\delta^3(\mathbf x-\mathbf y),\quad[A_\mu,A_\nu]=[\pi^\mu,\pi^\nu]=0.}
$$

These are identities of [operator-valued distributions](../../../../../../operator-valued-distribution.md), understood after smearing. The extra indices in the TeX polarization relation are transcription defects; the PDF has the ordinary two-polarization completeness contraction used above. The direct momenta of part (b) also satisfy the [canonical commutation relations](../../../../../../canonical-commutation-relation.md) after their boundary-generated shift, although they do not have the unmodified mode expansion printed here.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 301](../../../paper-301-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
