<h1 id="33a/solution">Solution</h1>

↑ **Parent:** [33A](../33a.md)

Use the [Minkowski metric](../../../../../minkowski-metric.md) with signature $(-,+,+,+)$. The source point is the intersection of the worldline with the observation event's past [light cone](../../../../../light-cone.md): $R^\mu R_\mu=0$ and $R^0>0$. In components this is $c(t-t_r)=|x-y(t_r)|$ with $t_r<t$. For a timelike worldline the retarded solution is unique in the usual complete-source setting.

Writing $R=|x-y(t_r)|$, $n=(x-y)/R$ and $u^\mu=\gamma(c,v)$ gives $R\cdot u=-\gamma cR(1-n\cdot v/c)$. Thus the [Liénard–Wiechert potentials](../../../../../lienard-wiechert-potential.md) are $\phi=q\mu_0c^2/[4\pi R(1-n\cdot v/c)]$ and $A=q\mu_0v/[4\pi R(1-n\cdot v/c)]$. At leading order in $1/r$ and first order in $v/c$, set $R\simeq r,n\simeq\hat r$ and expand the denominator:

$$
\phi\simeq\frac{q\mu_0c}{4\pi r}(c+\hat r\cdot v(t_r)),\qquad A\simeq\frac{q\mu_0}{4\pi r}v(t_r).
$$

Now use $t_-=t-r/c$ and let $a=\dot v(t_-)$. Derivatives of $1/r$ and $\hat r$ give near-field terms of order $r^{-2}$; the radiation terms come from $\partial_t t_-=1$ and $\nabla t_-=-\hat r/c$. The [electric field](../../../../../electric-field.md) and [magnetic field](../../../../../magnetic-field.md) are therefore

$$
\boxed{E=\frac{q\mu_0}{4\pi r}[\hat r(\hat r\cdot a)-a],\qquad B=-\frac{q\mu_0}{4\pi cr}\hat r\times a=\frac1c\hat r\times E.}
$$

They are transverse to the observation direction. The [Poynting vector](../../../../../poynting-vector.md) is

$$
\boxed{\frac1{\mu_0}E\times B=\frac{q^2\mu_0}{16\pi^2cr^2}\hat r\,|\hat r\times a|^2.}
$$

Integrating over a sphere uses $\int\sin^2\theta\,d\Omega=8\pi/3$, yielding the nonrelativistic [Larmor formula](../../../../../larmor-formula.md) $P=q^2\mu_0|a|^2/(6\pi c)$. For [simple harmonic motion](../../../../../simple-harmonic-motion.md), $|a|^2=A^2\omega^4\cos^2(\omega t_-)$, whose period average is $A^2\omega^4/2$. Multiplication by the period $2\pi/\omega$ gives

$$
\boxed{E_{\rm period}=q^2\mu_0A^2\omega^3/(6c).}
$$

This is the leading radiation energy in the nonrelativistic and far-field approximation.

## ↑ Ancestors (10)

1. [33A](../33a.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
