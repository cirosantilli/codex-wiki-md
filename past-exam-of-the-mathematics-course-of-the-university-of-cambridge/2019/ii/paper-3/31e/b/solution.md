<h1 id="31e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Keep the same function $V$. For arbitrary $a,b$ its [orbital derivative](../../../../../../orbital-derivative.md) is

$$
\dot V=r\{a x(x-1)-b y(y-1)\}.
$$

Let $\gamma$ be a nonconstant orbit of the unperturbed system with period $T$. Since

$$
\frac{\dot y}{ry}=x-1,
\qquad
\frac{\dot x}{x}=1-y,
$$

integration over one period gives

$$
\int_0^T(1-x)\,dt=0,
\qquad
\int_0^T(1-y)\,dt=0.
$$

Consequently,

$$
\begin{aligned}
A&:=\int_0^T x(x-1)\,dt
=\int_0^T(1-x)^2\,dt>0,\\
B&:=\int_0^T y(y-1)\,dt
=\int_0^T(1-y)^2\,dt>0.
\end{aligned}
$$

If a perturbed periodic orbit persisted and converged to $\gamma$ as $(a,b)\to(0,0)$, its net change in $V$ over one period would vanish. The [averaged first-integral obstruction to persistence of a periodic orbit](../../../../../../averaged-first-integral-obstruction-to-persistence-of-a-periodic-orbit.md) would therefore require

$$
0=r(aA-bB)+o(|a|+|b|).
$$

When $ab<0$, the two leading terms have the same nonzero sign and their magnitude is bounded below by $r\min(A,B)(|a|+|b|)$. **Thus no unperturbed periodic orbit persists for sufficiently small $a,b$ with $ab<0$.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [31E](../../31e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
