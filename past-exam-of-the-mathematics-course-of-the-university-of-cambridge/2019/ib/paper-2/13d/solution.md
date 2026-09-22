<h1 id="13d/solution">Solution</h1>

↑ **Parent:** [13D](../13d.md)

Let $v_1,v_2\ne0$ be tangent vectors to the two smooth curves at $p$. [complex differentiability at a point](../../../../../complex-differentiability-at-a-point.md) gives

$$
f(p+h)=f(p)+f'(p)h+o(|h|).
$$

When $f'(p)\ne0$, its real derivative is multiplication by a nonzero complex number, which is a rotation followed by a positive scaling. It therefore preserves the angle between $v_1$ and $v_2$, so $f$ is [conformal](../../../../../conformal-map.md) at $p$. The condition is essential: $f(z)=z^2$ has $f'(0)=0$ and sends rays making angle $\pi/4$ at zero to rays making angle $\pi/2$.

For $J(z)=z+z^{-1}$,

$$
J(z)=J(w)\quad\Longleftrightarrow\quad (z-w)(zw-1)=0.
$$

If $z,w$ both satisfy $|z|>1$, or both satisfy $0<|z|<1$, the alternative $zw=1$ is impossible unless the points lie on the omitted unit circle. Hence $J$ is one-to-one on each region. Also $J'(z)=1-z^{-2}$ has no zero there, so the restrictions are conformal. Solving $z^2-wz+1=0$ shows that $w\in[-2,2]$ exactly when both roots lie on the unit circle; otherwise one root is inside and the other outside. Thus each region has image

$$
\boxed{\mathbb C\setminus[-2,2]}.
$$

Taking the reciprocal of the interior restriction and filling its removable value at zero gives

$$
\boxed{g(z)=\frac1{J(z)}=\frac{z}{1+z^2}}.
$$

The reciprocal sends $\mathbb C\setminus[-2,2]$ onto

$$
\mathbb C\setminus\bigl(({-\infty},-1/2]\cup[1/2,\infty)\bigr),
$$

and $g(0)=0$. Therefore $g$ is the required one-to-one conformal map from the [unit disc](../../../../../unit-disc.md).

## ↑ Ancestors (10)

1. [13D](../13d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
