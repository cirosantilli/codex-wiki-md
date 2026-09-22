<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Identify the [circle group](../../../../../../circle-group.md) with $[0,1)$ modulo its endpoints, and let $\lambda$ be normalized [Lebesgue measure](../../../../../../lebesgue-measure.md). We first check invariance. On the $r$th inverse branch, $x=(y+r)/m$ for $0\leq r<m$. For an integrable [function](../../../../../../function-split.md) $g$, substitution gives

$$
\int_0^1g(E_mx)\,dx
=\sum_{r=0}^{m-1}\frac1m\int_0^1g(y)\,dy
=\int_0^1g(y)\,dy.
$$

In particular, testing [indicator functions](../../../../../../indicator-function.md) shows that the [integer multiplication map on the circle](../../../../../../integer-multiplication-map-on-the-circle.md) preserves $\lambda$.

To prove [ergodicity](../../../../../../ergodicity.md), let $B$ be a measurable set with $\lambda(E_m^{-1}B\mathbin{\triangle}B)=0$ and put $h=\mathbf1_B$. Then $h(E_mx)=h(x)$ almost everywhere. Its [Fourier coefficients](../../../../../../fourier-coefficient.md) are

$$
c_k=\int_0^1h(x)e^{-2\pi ikx}\,dx\qquad(k\in\mathbb Z).
$$

Using invariance of $h$ and substituting separately on the same $m$ branches gives

$$
\begin{aligned}
c_k
&=\int_0^1h(E_mx)e^{-2\pi ikx}\,dx\\
&=\frac1m\sum_{r=0}^{m-1}e^{-2\pi ikr/m}
  \int_0^1h(y)e^{-2\pi i(k/m)y}\,dy\\
&=\begin{cases}0,&m\nmid k,\\c_{k/m},&m\mid k.\end{cases}
\end{aligned}
$$

In the last line, the finite [geometric series](../../../../../../geometric-series.md) of $m$th [roots of unity](../../../../../../root-of-unity.md) is zero unless $m$ divides $k$, when it equals $m$. For any nonzero integer $k$, divide repeatedly by $m$ until the resulting integer is no longer divisible by $m$. The recurrence then implies $c_k=0$.

Since the [Fourier basis](../../../../../../fourier-basis.md) is a complete [orthonormal basis](../../../../../../orthonormal-basis.md) of $L^2([0,1),\lambda)$, the absence of every nonconstant [Fourier coefficient](../../../../../../fourier-coefficient.md) implies $h=c_0=\lambda(B)$ almost everywhere. An [indicator function](../../../../../../indicator-function.md) takes only the values zero and one, so $\lambda(B)$ must be zero or one. This proves

$$
\boxed{E_m\text{ is ergodic for Lebesgue measure for every integer }m\geq2.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
