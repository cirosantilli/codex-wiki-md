<h1 id="9b/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For the [barotropic equation of state](../../../../../../barotropic-equation-of-state.md) $P=w\rho$, the continuity equation separates as

$$
\frac{d\rho}{\rho}=-3(1+w)\frac{da}{a}.
$$

Since $a(t_0)=1$,

$$
\rho=\rho_0a^{-3(1+w)},
\qquad \rho_0=\rho(t_0),
$$

which is the [constant-equation-of-state density scaling](../../../../../../constant-equation-of-state-density-scaling.md).

When $Q=0$, the expanding branch satisfies

$$
\dot a=\sqrt{\frac{8\pi G\rho_0}{3c^2}}
 a^{-(1+3w)/2}=H_0a^{-(1+3w)/2},
$$

where $H_0=\dot a(t_0)>0$. Because $w>-1$, integration gives

$$
a(t)^{3(1+w)/2}
=1+\frac32(1+w)H_0(t-t_0),
$$

and hence the [flat constant-equation-of-state scale factor](../../../../../../flat-constant-equation-of-state-scale-factor.md)

$$
\boxed{
a(t)=\left[1+\frac32(1+w)H_0(t-t_0)\right]^{2/[3(1+w)]}
}.
$$

It vanishes at

$$
\boxed{t_*=t_0-\frac{2}{3(1+w)H_0}<t_0},
$$

as $|w|<1$ ensures $1+w>0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [9B](../../9b.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
