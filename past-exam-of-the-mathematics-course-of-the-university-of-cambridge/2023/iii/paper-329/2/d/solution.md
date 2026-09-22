<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let

$$
\delta=(ah_0)^{1/2},
\qquad
\xi=\frac{x-L}{\delta},
\qquad
H=\frac h{h_0},
\qquad
V=\frac{\mu U}{\gamma}\left(\frac a{h_0}\right)^{1/2}.
$$

Flux conservation gives $u=U/H$. Substitution into the extensional-force equation yields the third-order equation

$$
\boxed{HH_{\xi\xi\xi}
-4V(H^{-1}H_\xi)_\xi=0}.
$$

Since

$$
HH_{\xi\xi\xi}
=\left(HH_{\xi\xi}-\frac12H_\xi^2\right)_\xi,
$$

one integration, using $H\to1$ and its derivatives tending to zero on the flat-film side, gives

$$
HH_{\xi\xi}-\frac12H_\xi^2
=4V\frac{H_\xi}{H}.
$$

Put $q(H)=H_\xi$. After division by $q$, this becomes

$$
H\frac{dq}{dH}-\frac12q=\frac{4V}{H}.
$$

The [integrating factor](../../../../../../integrating-factor.md) $H^{-1/2}$ gives

$$
\frac d{dH}(qH^{-1/2})=4VH^{-5/2}.
$$

A second integration and $q(1)=0$ therefore give

$$
\boxed{H^{-1/2}H_\xi
=\frac{8V}{3}(1-H^{-3/2})}.
$$

On the bubble side, matching to its cylindrical shape gives $H\sim\xi^2/2$, so $H^{-1/2}H_\xi\to\sqrt2$. Taking $H\to\infty$ in the integrated equation yields $8V/3=\sqrt2$. Hence

$$
\boxed{
U=\frac{3\gamma}{8\mu}
\left(\frac{2h_0}{a}\right)^{1/2}}.
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 329](../../../paper-329-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
