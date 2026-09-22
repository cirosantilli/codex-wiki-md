<h1 id="1/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

At late time $f(k,\tau_0)\to H/\sqrt{2k^3}$ and $a=-1/(H\tau)$. Define the [elementary symmetric polynomials](../../../../../../elementary-symmetric-polynomial.md)

$$
e_2=\sum_{a<b}k_ak_b,
\qquad e_3=\sum_{a<b<c}k_ak_bk_c,
\qquad e_4=k_1k_2k_3k_4.
$$

Then part ii reduces to

$$
\langle O\rangle'_\lambda
=-\frac{i\lambda H^4\mathcal E}{8\prod_a k_a^3}\operatorname{Im}J(\tau_0),
$$

where a prime removes the momentum-conserving [Dirac delta distribution](../../../../../../dirac-delta-function.md) and

$$
J(\tau_0)=\int_{-\infty(1-i\epsilon)}^{\tau_0}
\frac{d\tau}{\tau^4}e^{-ik_T\tau}
\prod_{a=1}^4(1+ik_a\tau).
$$

Expanding the product gives

$$
\frac1{\tau^4}\prod_a(1+ik_a\tau)
=\frac1{\tau^4}+\frac{ik_T}{\tau^3}-\frac{e_2}{\tau^2}
-\frac{ie_3}{\tau}+e_4.
$$

Repeated [integration by parts](../../../../../../integration-by-parts.md) reduces every negative power to the supplied logarithmic integral. The power divergences are real and disappear when the imaginary part is taken. Writing

$$
L_T=\gamma_E+\log|k_T\tau_0|,
$$

one obtains

$$
\operatorname{Im}J
=\left(-\frac{k_T^3}{3}+k_Te_2-e_3\right)L_T
+\frac{4k_T^3}{9}-k_Te_2+\frac{e_4}{k_T}+o(1).
$$

Consequently the late-time [parity-odd primordial trispectrum](../../../../../../parity-odd-primordial-trispectrum.md) is

$$
\boxed{
\langle\phi_1(\mathbf k_1)\phi_2(\mathbf k_2)
\phi_3(\mathbf k_3)\phi_4(\mathbf k_4)\rangle'
=-\frac{i\lambda H^4}{8\prod_a k_a^3}
[\mathbf k_2\mathbin\cdot(\mathbf k_3\mathbin\times\mathbf k_4)]
\left[
\left(-\frac{k_T^3}{3}+k_Te_2-e_3\right)L_T
+\frac{4k_T^3}{9}-k_Te_2+\frac{e_4}{k_T}
\right]}.
$$

Its factor of $i$ is required by [reality of a momentum-space scalar correlator](../../../../../../reality-of-a-momentum-space-scalar-correlator.md): reversing all momenta complex-conjugates the correlator, while the [scalar triple product](../../../../../../scalar-triple-product.md) changes sign.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
