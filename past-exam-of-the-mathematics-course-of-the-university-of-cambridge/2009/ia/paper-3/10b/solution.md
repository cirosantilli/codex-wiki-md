<h1 id="10b/solution">Solution</h1>

↑ **Parent:** [10B](../10b.md)

For a twice differentiable [vector potential](../../../../../vector-potential.md) $\mathbf B$, commuting partial derivatives in $\mathbf J=\nabla\times\mathbf B$ gives the necessary condition

$$
\boxed{\nabla\cdot\mathbf J=0.}
$$

The potential is not unique: for any sufficiently smooth scalar $\psi$, $\mathbf B+\nabla\psi$ has the same [curl](../../../../../curl.md), since the [curl of a gradient](../../../../../curl-of-a-gradient.md) is zero. This is the usual [gradient](../../../../../gradient.md) freedom of a [vector potential](../../../../../vector-potential.md). A divergence-free condition alone need not suffice globally on every domain; here only its necessity is requested.

[Stokes theorem](../../../../../stokes-theorem.md) states that for an oriented surface with compatible boundary orientation,

$$
\int_S(\nabla\times\mathbf B)\cdot\mathbf n\,dS
=\oint_{\partial S}\mathbf B\cdot d\mathbf r.
$$

For the integrand in this problem, a convenient globally smooth [vector potential](../../../../../vector-potential.md) is

$$
\mathbf B=\frac13(z^3,x^3,y^3),\qquad
\nabla\times\mathbf B=(y^2,z^2,x^2).
$$

The boundary of the upper ellipsoid is the ellipse $z=0$. The outward normal on the upper surface induces counterclockwise orientation viewed from above, so parameterize it as $\mathbf r(\theta)=(a\cos\theta,b\sin\theta,0)$, $0\leq\theta\leq2\pi$. Along this curve the first component of $\mathbf B$ is zero and $dz=0$, leaving

$$
\oint\mathbf B\cdot d\mathbf r
=\frac13\int_0^{2\pi}(a\cos\theta)^3 b\cos\theta\,d\theta
=\frac{a^3b}{3}\int_0^{2\pi}\cos^4\theta\,d\theta.
$$

Since the last angular integral is $3\pi/4$,

$$
\boxed{\int_S(y^2,z^2,x^2)\cdot d\mathbf A=\frac{\pi a^3b}{4}.}
$$

The result is independent of the vertical semiaxis $c$. As a sign check, the field is divergence-free, so closing the cap with the downward-oriented base disc makes its flux the positive integral of $x^2$ over that disc, which has the same value.

## ↑ Ancestors (10)

1. [10B](../10b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
