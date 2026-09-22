<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [mass shell](../../../../../../mass-shell.md) constraint and the conserved [comoving momentum](../../../../../../comoving-momentum.md) give

$$
\frac{dt}{ds}=\sqrt{1+\frac{(p^C)^2}{m^2a^2}},\qquad \frac{d\mathbf x}{ds}=\frac{\mathbf p^C}{ma^2}.
$$

Dividing yields

$$
\boxed{\frac{d\mathbf x}{dt}=\frac{\mathbf p^C}{a\sqrt{(p^C)^2+m^2a^2}}.}
$$

The comoving direction is constant because $\mathbf p^C$ is constant. With $a(t_0)=1$ and physical [momentum](../../../../../../momentum.md) magnitude $p_0>0$ at $t_0$, we have $p^C=p_0$. Integrating the speed along that fixed direction gives

$$
\boxed{d=\int_0^{t_0}\frac{dt}{a(t)}\frac1{\sqrt{1+[ma(t)/p_0]^2}}.}
$$

This is a distance travelled, rather than a light-ray distance: the extra factor is the particle's proper peculiar speed $v=p^K/\sqrt{m^2+(p^K)^2}$. For a particle at rest, $p_0=0$, the distance is zero, understood separately or as the limit. The formula assumes collisionless motion over the interval. Its existence at the lower endpoint depends on the early [scale factor](../../../../../../scale-factor-cosmology.md); in [radiation domination](../../../../../../radiation-domination.md) the integral is finite.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
