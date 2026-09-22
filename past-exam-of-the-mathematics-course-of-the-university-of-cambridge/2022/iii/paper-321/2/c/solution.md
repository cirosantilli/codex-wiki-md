<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Inside the ring, $\nu\Sigma=A\Sigma^3=A\sigma^3(1-x^2/w^2)^{3/2}$. Part a therefore gives

$$
\boxed{u_x=\frac{9A\sigma^2}{w^2}x}.
$$

The edge is material, so $\dot w=u_x(w)$ and

$$
\boxed{\dot w=\frac{9A\sigma^2}{w}}.
$$

Direct substitution of the profile into the diffusion equation gives

$$
\boxed{\dot\sigma=-\frac{\sigma\dot w}{w}},
$$

hence $\sigma w=\sigma_0w_0$. This is exactly [mass conservation](../../../../../../mass-conservation.md), since

$$
M_{\rm ring}=\int_{-w}^w\Sigma\,dx
=\sigma w\int_{-1}^1\sqrt{1-y^2}\,dy
=\frac\pi2\sigma w.
$$

Using $\sigma=\sigma_0w_0/w$ in the width equation and integrating,

$$
w^4=w_0^4+36A\sigma_0^2w_0^2t.
$$

Therefore

$$
\boxed{
w=w_0\left(1+\frac{36A\sigma_0^2}{w_0^2}t\right)^{1/4},
\qquad
\sigma=\sigma_0\left(1+\frac{36A\sigma_0^2}{w_0^2}t\right)^{-1/4}}.
$$

In particular, $w\propto t^{1/4}$ at late times.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 321](../../../paper-321-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
