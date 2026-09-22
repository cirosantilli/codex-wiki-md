<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a uniform sphere of radius $R$, write $M(r)=M(r/R)^3$ and $dM=3Mr^2dr/R^3$. The self-gravitational [potential energy](../../../../../../potential-energy.md) is assembled by adding shells:

$$
U_G=-\int_0^R\frac{GM(r)}r\,dM(r)
=-\frac{3GM^2}{R^6}\int_0^Rr^4\,dr
=-\frac{3GM^2}{5R}.
$$

The [cosmological constant](../../../../../../cosmological-constant.md) produces the external potential per unit mass $\Phi_\Lambda=-\Lambda r^2/6$, since $-\nabla\Phi_\Lambda=\Lambda\mathbf r/3$ in units $c=1$. Its energy is

$$
U_\Lambda=\int_0^R\Phi_\Lambda\,dM=-\frac{\Lambda}{6}\frac{3M}{R^3}\int_0^Rr^4\,dr=-\frac{\Lambda MR^2}{10}.
$$

There is no additional factor $1/2$ for this fixed external potential, unlike the pair-counting factor for gravitational self-energy. At the maximum radius $R=r_m$, the kinetic energy vanishes, so

$$
\boxed{U_m=-\frac35\frac{GM^2}{r_m}-\frac1{10}\Lambda Mr_m^2.}
$$

This is the turnaround energy in [uniform-sphere collapse with a cosmological constant](../../../../../../uniform-sphere-collapse-with-a-cosmological-constant.md). The original PDF's shell kinetic term is $\dot r^2/2$, not the $r^2/2$ produced by the TeX transcription.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 45](../../../paper-45-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
