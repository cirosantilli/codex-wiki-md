<h1 id="36b/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $R=|\mathbf x|$, $\widehat{\mathbf R}=\mathbf x/R$, and $t_R=t-R/c$. To leading nonzero [multipole expansion](../../../../../../electromagnetic-multipole-expansion.md) order, the loop is a time-dependent [magnetic dipole](../../../../../../magnetic-dipole-moment.md) with

$$
\mathbf m(t)=\pi r^2I(t)\mathbf n.
$$

Expanding the [retarded electromagnetic potential](../../../../../../retarded-potential.md) across the small loop gives

$$
\mathbf A(\mathbf x,t)
=\frac{\mu_0}{4\pi}
\left[
\frac{\mathbf m(t_R)\times\widehat{\mathbf R}}{R^2}
+\frac{\dot{\mathbf m}(t_R)\times\widehat{\mathbf R}}{cR}
\right]
+O\!\left(\frac{r^3}{R^3}\right).
$$

The $R^{-2}$ term is the near magnetic-dipole field and the $R^{-1}$ term is the [magnetic dipole radiation](../../../../../../magnetic-dipole-radiation.md) field. Substituting the Fourier series for the current gives

$$
\boxed{
\mathbf A(\mathbf x,t)
=\frac{\mu_0r^2}{4}
(\mathbf n\times\widehat{\mathbf R})
\sum_{n=0}^{\infty}I_n
\left[
\frac{\sin(n\omega t_R)}{R^2}
+\frac{n\omega}{cR}\cos(n\omega t_R)
\right]
}.
$$

The $n=0$ summand vanishes for the stated sine series.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [36B](../../36b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
