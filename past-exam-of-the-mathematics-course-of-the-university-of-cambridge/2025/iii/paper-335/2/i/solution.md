<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

With the [scattering potential](../../../../../../scattering-potential.md) $V(\mathbf r)=k_0^2(1-n^2(\mathbf r))$, the total field obeys

$$
(\nabla^2+k_0^2)\psi=V\psi.
$$

The outgoing Green function is $G_0(\mathbf r)=e^{ik_0|\mathbf r|}/(4\pi|\mathbf r|)$. The [Lippmann-Schwinger equation](../../../../../../lippmann-schwinger-equation.md) and the first [Born approximation](../../../../../../born-approximation.md) give

$$
\psi_s(\mathbf r)simeq
-\int_DG_0(\mathbf r-\mathbf r')V(\mathbf r')
e^{ik_0\widehat{\mathbf x}_0\cdot\mathbf r'},d\mathbf r'.
$$

For $r\to\infty$,

$$
G_0(\mathbf r-\mathbf r')
\sim\frac{e^{ik_0r}}{4\pi r}
e^{-ik_0\widehat{\mathbf r}\cdot\mathbf r'},
$$

so

$$
\boxed{
\psi_s(\mathbf r)\sim\frac{e^{ik_0r}}r
f_\infty(\widehat{\mathbf x}_0,\widehat{\mathbf r}),
\qquad
f_\infty=-\frac1{4\pi}
\int_DV(\mathbf r')e^{-i\mathbf q\cdot\mathbf r'}d\mathbf r',}
$$

where $\mathbf q=k_0(\widehat{\mathbf r}-\widehat{\mathbf x}_0)$ is the [momentum transfer](../../../../../../momentum-transfer.md). Thus the [far-field pattern](../../../../../../far-field-pattern.md) is $-1/(4\pi)$ times the Fourier transform of $V$ at the measured transfer vectors. If sufficiently many incident directions and frequencies supply all $\mathbf q$, the formal reconstruction is

$$
\boxed{V(\mathbf r)=-4\pi\mathcal F^{-1}
\{f_\infty(\mathbf q)\}(\mathbf r),}
$$

with constants adjusted to the chosen Fourier convention.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
