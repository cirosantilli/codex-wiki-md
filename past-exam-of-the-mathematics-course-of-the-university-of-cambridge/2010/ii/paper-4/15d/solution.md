<h1 id="15d/solution">Solution</h1>

↑ **Parent:** [15D](../15d.md)

For a canonical coordinate and momentum, the [Poisson bracket](../../../../../poisson-bracket.md) is

$$
\{f,g\}=f_qg_p-f_pg_q.
$$

The chain rule and [Hamilton equations](../../../../../hamilton-s-equations.md) $\dot q=H_p$, $\dot p=-H_q$ give

$$
\boxed{\frac{df}{dt}=\{f,H\}+f_t.}
$$

For the stated complex variables, direct differentiation gives

$$
\{a,a\}=0,\qquad
\boxed{\{a,a^*\}=-i.}
$$

Since $H=\omega aa^*$, the product rule for the [Poisson bracket](../../../../../poisson-bracket.md) yields

$$
\{a,H\}=-i\omega a,\qquad \{a^*,H\}=i\omega a^*.
$$

The linear change of variables is invertible, so treating $a,a^*$ as independent coordinates when differentiating gives

$$
\boxed{\frac{df}{dt}
=i\omega\left(a^*\frac{\partial f}{\partial a^*}
-a\frac{\partial f}{\partial a}\right)+\frac{\partial f}{\partial t}.}
$$

In particular $a(t)=a(0)e^{-i\omega t}$ and $a^*(t)=a^*(0)e^{i\omega t}$. On a continuously chosen branch along a nonzero trajectory,

$$
\boxed{\log a^*-i\omega t,\qquad \log a+i\omega t}
$$

are constant. The logarithm is undefined at the zero-energy equilibrium, and a fixed principal branch need not be continuous across its cut; the branch qualification is necessary.

## ↑ Ancestors (10)

1. [15D](../15d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
