<h1 id="1/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Assume a real [refractive index](../../../../../../../refractive-index.md) and write the [scattering potential](../../../../../../../scattering-potential.md) as $V=\langle V\rangle+W$, so $\langle W\rangle=0$ by construction. With the real kernel components in the question, the logarithmic [Rytov approximation](../../../../../../../rytov-approximation.md) separates into

$$
\operatorname{Re}\chi_1=-\int a(\mathbf r,\mathbf r')V(\mathbf r')\,d\mathbf r',\qquad \operatorname{Im}\chi_1=-\int b(\mathbf r,\mathbf r')V(\mathbf r')\,d\mathbf r'.
$$

Include the incident [wave phase](../../../../../../../phase-waves.md) and the mean-potential [wave phase](../../../../../../../phase-waves.md) in the deterministic reference $\phi_0$: at each observation point it is $\arg\psi_i-\int b\langle V\rangle$. It need not be spatially constant. The [amplitude](../../../../../../../wave-amplitude.md) is $|\psi_i|\exp[-\int aV]$. The [phase covariance in the first Rytov approximation](../../../../../../../phase-covariance-in-the-first-rytov-approximation.md) therefore starts from the fluctuating [wave phase](../../../../../../../phase-waves.md)

$$
\boxed{\varphi(\mathbf r)=-\int b(\mathbf r,\mathbf r')W(\mathbf r')\,d\mathbf r'.}
$$

Under the integrability assumptions needed to interchange the expectation and integral,

$$
\boxed{\langle\varphi(\mathbf r)\rangle=-\int b(\mathbf r,\mathbf r')\langle W(\mathbf r')\rangle\,d\mathbf r'=0.}
$$

For a complex absorbing potential, the corresponding phase fluctuation is $-\int[b\operatorname{Re}W+a\operatorname{Im}W]$; the displayed scalar formula is the real-index case. The zero mean comes from centering $V$, not from setting the mean of $V$ equal to zero. In particular the printed $\langle n\rangle=0$ does not imply $\langle V\rangle=0$. A physical positive [refractive index](../../../../../../../refractive-index.md) usually has a nonzero background mean; a zero-mean assumption normally refers to its fluctuation. The algebra above remains meaningful for a signed real random field and explicitly retains its mean [scattering potential](../../../../../../../scattering-potential.md).

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 72](../../../../paper-72-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
