<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use the leading far-field kernel from the previous part. Define

$$
\Phi=k_0(r-\widehat{\mathbf r}_0\cdot\mathbf r),\qquad \mathbf q=k_0(\widehat{\mathbf r}_0-\widehat{\mathbf r}),\qquad K(\mathbf r')=\frac{e^{i(\Phi+\mathbf q\cdot\mathbf r')}}{4\pi r}.
$$

Then $\phi_1=\int_D K V$ and, because the incident intensity is one,

$$
I=\mathbb E\exp(\phi_1+\overline\phi_1)=\mathbb E\exp\left[\int_D a(\mathbf r')V(\mathbf r')\,d\mathbf r'\right],\qquad a(\mathbf r')=\frac{\cos(\Phi+\mathbf q\cdot\mathbf r')}{2\pi r}.
$$

To first order in weak contrast, $V=2\mu k_0^2W+O(\mu^2)$. Its linearized part is a centered [stationary Gaussian random field](../../../../../../stationary-gaussian-random-field.md), with [autocorrelation function of a random field](../../../../../../autocorrelation-function-of-a-random-field.md) $C_V(\mathbf s)=4\mu^2k_0^4C_W(\mathbf s)$. The [exponential moment of a Gaussian linear functional](../../../../../../exponential-moment-of-a-gaussian-linear-functional.md) therefore gives the usual [Gaussian intensity in the first Rytov approximation](../../../../../../gaussian-intensity-in-the-first-rytov-approximation.md):

$$
\boxed{I=\exp\left[\frac1{8\pi^2r^2}\int_D\int_D C_V(\mathbf r'-\mathbf r'')\cos(\Phi+\mathbf q\cdot\mathbf r')\cos(\Phi+\mathbf q\cdot\mathbf r'')\,d\mathbf r'\,d\mathbf r''\right].}
$$

Equivalently the exponent is $\mathbb E|\phi_1|^2+\operatorname{Re}\mathbb E\phi_1^2$. The second term generally matters because a finite real random medium need not generate a circular complex Gaussian amplitude.

If the full stated potential $V=k_0^2(2\mu W+\mu^2W^2)$ is retained, it is not Gaussian and has mean $m_V=\mu^2k_0^2$. To retain every term through order $\mu^2$ in the intensity of this first Rytov field, the cumulant expansion instead gives

$$
\boxed{\log I=m_V\int_Da(\mathbf r')\,d\mathbf r'+\frac12\int_D\int_D a(\mathbf r')a(\mathbf r'')C_V^{\rm cov}(\mathbf r'-\mathbf r'')\,d\mathbf r'\,d\mathbf r''+O(\mu^4).}
$$

Here $C_V^{\rm cov}=\mathbb E[(V-m_V)(V'-m_V)]$; the raw autocorrelation differs by $m_V^2=O(\mu^4)$. The stated remainder uses Gaussian finite-dimensional statistics of $W$, for which odd total moments vanish. This mean term is absent if one first truncates the potential to $2\mu k_0^2W$. Both formulas concern the first Rytov approximation, and exponentiating it does not supply the omitted higher-order scattering corrections.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
