<h1 id="16a/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At the moving boundary,

$$
Q=4\pi a^2\dot a.
$$

Substitution into the result of part (b) gives the [Rayleigh collapse equation](../../../../../../rayleigh-collapse-of-a-spherical-cavity.md)

$$
a\ddot a+\frac32\dot a^2=-\frac{p_0}{\rho}.
$$

Treat $v=\dot a$ as a function of $a$, so that $\ddot a=v\,dv/da$. With $w=v^2$, the equation becomes

$$
a\frac{dw}{da}+3w=-\frac{2p_0}{\rho}.
$$

Multiplication by the [integrating factor](../../../../../../integrating-factor.md) $a^3$ after division by $a$ gives

$$
\frac d{da}(a^3w)=-\frac{2p_0}{\rho}a^2.
$$

Using $w(a_0)=0$,

$$
w(a)=\frac{2p_0}{3\rho}
\left(\frac{a_0^3}{a^3}-1\right).
$$

The collapsing branch has negative radial velocity, so

$$
\boxed{
\dot a=-\sqrt{\frac{2p_0}{3\rho}
\left(\frac{a_0^3}{a^3}-1\right)}
}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [16A](../../16a.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
