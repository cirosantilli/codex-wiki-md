<h1 id="1/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For a [Keplerian orbit](../../../../../../../kepler-orbit.md), write $h=Kr^{1/2}$, so $h'=h/(2r)$. Substituting the stated torque laws into

$$
\partial_r\mathcal G-r\mathcal T=\dot Mh'
$$

gives

$$
y'+\left(\frac1{2r}-\frac{\beta}{3\nu r^{1/2}}\right)y
=\frac{\dot M}{6\pi r}.
$$

With

$$
x=\frac r{r_{\rm in}},
\qquad
\lambda=-\frac{2\beta\sqrt{r_{\rm in}}}{3\nu},
$$

the [integrating factor](../../../../../../../integrating-factor.md) is $x^{1/2}e^{\lambda\sqrt x}$. The boundary condition $y(1)=0$ then gives

$$
y(x)=\frac{\dot M}{3\pi\lambda}x^{-1/2}
\left[1-e^{\lambda(1-\sqrt x)}\right].
$$

Thus

$$
\boxed{f(x)=1-\sqrt x}
$$

and

$$
\boxed{\nu\Sigma
=\frac{\dot M}{3\pi\lambda}x^{-1/2}
[1-\exp(\lambda f(x))]}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 321](../../../../paper-321-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
