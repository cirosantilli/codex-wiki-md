<h1 id="4/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use the [Fourier transform](../../../../../../../fourier-transform.md) convention $\zeta(\mathbf x)=\int d^3k\,e^{i\mathbf k\cdot\mathbf x}\zeta(\mathbf k)/(2\pi)^3$. Statistical homogeneity and isotropy define the [primordial bispectrum](../../../../../../../primordial-bispectrum.md) by

$$
\boxed{\langle\zeta(\mathbf k_1)\zeta(\mathbf k_2)\zeta(\mathbf k_3)\rangle_c=(2\pi)^3\delta^{(3)}(\mathbf k_1+\mathbf k_2+\mathbf k_3)B(k_1,k_2,k_3).}
$$

The [Dirac delta function](../../../../../../../dirac-delta-function.md) enforces [momentum conservation](../../../../../../../momentum-conservation.md); the three magnitudes describe a closed triangle. Set $\alpha=3f_{\mathrm{NL}}/5$. For the [centered quadratic Gaussian transformation](../../../../../../../centered-quadratic-gaussian-transformation.md), its quadratic Fourier term is

$$
\alpha\int\frac{d^3q}{(2\pi)^3}G(\mathbf q)G(\mathbf k-\mathbf q)-\alpha(2\pi)^3\delta^{(3)}(\mathbf k)\langle G^2\rangle.
$$

At first order in $\alpha$, choose the quadratic field at one of the three external positions. For the first position, [Wick contractions](../../../../../../../wick-contraction.md) pair the two internal fields with the two remaining external fields in two ways. The self-pairing is precisely removed by the subtracted mean. The surviving contribution is $2\alpha P(k_2)P(k_3)$ times the momentum delta. Adding the other positions gives the tree-level [local-type primordial non-Gaussianity](../../../../../../../local-type-primordial-non-gaussianity.md) result

$$
\boxed{B^{\mathrm{loc}}=\frac65f_{\mathrm{NL}}[P(k_1)P(k_2)+P(k_2)P(k_3)+P(k_3)P(k_1)].}
$$

**This expression is at leading order in $f_{\mathrm{NL}}$.** The exact quadratic map also has a [loop correction to the local primordial bispectrum](../../../../../../../loop-correction-to-the-local-primordial-bispectrum.md), from three quadratic vertices:

$$
B_{\mathrm{loop}}=8\alpha^3\int\frac{d^3q}{(2\pi)^3}P(q)P(|\mathbf k_1-\mathbf q|)P(|\mathbf k_2+\mathbf q|).
$$

There is no quadratic-in-$\alpha$ bispectrum term, because it would involve five centered Gaussian fields. A regulator may be needed for this higher-order integral. The displayed leading formula uses the Gaussian power $P$, consistently neglecting its order-$f_{\mathrm{NL}}^2$ correction.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [4](../../../4.md)
4. [Paper 312](../../../../paper-312-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
