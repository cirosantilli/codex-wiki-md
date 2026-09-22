<h1 id="30d/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Factor the integrand in the [Schläfli contour integral for Legendre polynomials](../../../../../../../schlafli-contour-integral-for-legendre-polynomials.md) as

$$
\frac{(z^2-1)^n}{(z-t)^{n+1}}
=\frac1{z-t}
\left(\frac{z^2-1}{z-t}\right)^n.
$$

Thus one may take

$$
f(z,t)=\frac1{z-t},
\qquad
\phi(z,t)=\log\left(\frac{z^2-1}{z-t}\right),
$$

with a branch of the logarithm chosen locally along the deformed contour. Differentiation gives

$$
\phi'(z,t)
=\frac{2z}{z^2-1}-\frac1{z-t}
=\frac{z^2-2tz+1}{(z^2-1)(z-t)}.
$$

For $t=\cos\theta$, its saddle points solve

$$
z^2-2(\cos\theta)z+1=0,
$$

and hence

$$
\boxed{z_\pm=\cos\theta\pm i\sin\theta=e^{\pm i\theta}}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [30D](../../../30d.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
