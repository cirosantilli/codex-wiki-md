<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the stationary [scattering potential](../../../../../../../scattering-potential.md) fluctuation have [autocorrelation function of a random field](../../../../../../../autocorrelation-function-of-a-random-field.md)

$$
C_W(\boldsymbol\rho)=\langle W(\mathbf r')W(\mathbf r'+\boldsymbol\rho)\rangle.
$$

Because $W$ is centered, this is also its [covariance function](../../../../../../../covariance-function.md). Multiplying the two real [wave phase](../../../../../../../phase-waves.md) integrals and taking expectations gives

$$
\boxed{\langle\varphi(\mathbf r)^2\rangle=\iint b(\mathbf r,\mathbf r')b(\mathbf r,\mathbf r'')C_W(\mathbf r''-\mathbf r')\,d\mathbf r'\,d\mathbf r''.}
$$

The two minus signs cancel. This is the [wave phase](../../../../../../../phase-waves.md) [variance](../../../../../../../variance-split.md), since the [wave phase](../../../../../../../phase-waves.md) mean is zero. More generally the [phase covariance in the first Rytov approximation](../../../../../../../phase-covariance-in-the-first-rytov-approximation.md) replaces the first kernel by $b(\mathbf r_1,\mathbf r')$ and the second by $b(\mathbf r_2,\mathbf r'')$. Finite observation/scattering windows, or suitable weighted-integrability hypotheses, make these double integrals well-defined in a stationary infinite-medium model.

The correlation needed here is that of the [scattering potential](../../../../../../../scattering-potential.md) fluctuation. With the printed $V=n^2-1$, the [covariance of a squared random field](../../../../../../../covariance-of-a-squared-random-field.md) is

$$
C_W(\boldsymbol\rho)=\langle n(\mathbf r')^2n(\mathbf r'+\boldsymbol\rho)^2\rangle-\langle n^2\rangle^2.
$$

It involves a fourth moment of $n$, so its value is not generally determined by the ordinary two-point correlation $C_n=\langle n(\mathbf r')n(\mathbf r'+\boldsymbol\rho)\rangle$ alone. If one additionally assumes a zero-mean [Gaussian random field](../../../../../../../gaussian-random-field.md), [Isserlis theorem](../../../../../../../isserlis-s-theorem.md) yields $C_W=2C_n^2$. That assumption is not printed and must not be inserted silently. Alternatively, for a physical weak fluctuation $n_{\rm phys}=1+\eta$, $W\simeq2\eta$ gives $C_W\simeq4C_\eta$. **The general answer uses $C_W$; either reduction to a [refractive index](../../../../../../../refractive-index.md) two-point correlation requires an extra assumption.**

## ↑ Ancestors (12)

1. [Ii](../ii.md)
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
