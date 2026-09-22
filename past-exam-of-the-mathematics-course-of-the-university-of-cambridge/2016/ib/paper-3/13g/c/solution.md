<h1 id="13g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For every closed piecewise smooth curve $\gamma$ in $U$, the [winding number](../../../../../../winding-number.md) of $f\circ\gamma$ about zero is the integer

$$
m_\gamma=\frac1{2\pi i}\int_\gamma\frac{f'(z)}{f(z)}\,dz.
$$

If $f=g_k^k$ for a holomorphic $k$th root, $g_k$ is nowhere zero, and

$$
m_\gamma=k\frac1{2\pi i}\int_\gamma\frac{g_k'}{g_k}\,dz.
$$

Thus $m_\gamma$ is divisible by every $k$ for which a root exists. An infinite subset of the positive integers is unbounded, so a fixed integer divisible by all those $k$ must be zero. Hence **all periods of the holomorphic function $f'/f$ vanish**.

Fix $z_0\in U$. Since a domain is connected and open, its points can be joined by piecewise smooth paths. Vanishing periods make

$$
H(z)=\int_{z_0}^{z}\frac{f'(w)}{f(w)}\,dw
$$

independent of path. It is a [holomorphic primitive](../../../../../../holomorphic-primitive.md) with $H'=f'/f$. Differentiating gives $(fe^{-H})'=0$, so $fe^{-H}=f(z_0)$. Choose a complex number $c$ with $e^c=f(z_0)$. Then

$$
\boxed{F=H+c\text{ is holomorphic on }U,\qquad f=e^F.}
$$

This constructs a global [holomorphic logarithm](../../../../../../holomorphic-logarithm.md) without requiring $U$ to be simply connected.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [13G](../../13g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
