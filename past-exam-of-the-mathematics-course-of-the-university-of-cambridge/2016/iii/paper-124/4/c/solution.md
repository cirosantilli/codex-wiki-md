<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $P(t)=\sum_{n\le\sqrt{t/(2\pi)}}n^{-1/2-it}$. The given bound for the [Riemann zeta function](../../../../../../riemann-zeta-function.md), together with $(a+b)^4\le8(a^4+b^4)$ for $a,b\ge0$, gives

$$
\int_1^T|\zeta(1/2+it)|^4\,dt\ll\int_1^T|P(t)|^4\,dt+\log T.
$$

The integral over $[0,1]$ is bounded, since the [Riemann zeta function](../../../../../../riemann-zeta-function.md) has no [pole](../../../../../../pole.md) on this compact segment. It remains to estimate the [fourth moment of the Riemann zeta function](../../../../../../fourth-moment-of-the-riemann-zeta-function.md) through this moving [Dirichlet polynomial](../../../../../../dirichlet-polynomial.md) cutoff.

Let $L=\lfloor\sqrt{T/(2\pi)}\rfloor$ and $Y=L^2$. In the expansion of $|P(t)|^4$, a quadruple $n_1,n_2,n_3,n_4\le L$ occurs precisely for

$$
t\ge t_0=\max\bigl(1,2\pi n_1^2,2\pi n_2^2,2\pi n_3^2,2\pi n_4^2\bigr).
$$

Its oscillatory factor is $e^{it\log(n_3n_4/(n_1n_2))}$, and its weight is $(n_1n_2n_3n_4)^{-1/2}$. When $n_1n_2=n_3n_4$, its integral has length at most $T$. When these products differ, its integral over $[t_0,T]$ has absolute value at most $2/|\log(n_3n_4/(n_1n_2))|$. Thus the moving cutoff affects the lower endpoint but preserves the off-diagonal bound from part (a).

Write $r_L(m)=\#\{(a,b):a,b\le L,\ ab=m\}$. The [divisor function](../../../../../../divisor-function.md) $d(m)$ bounds $r_L(m)$. Grouping the off-diagonal majorant by the two products and using the weighted row-sum argument in part (a), with coefficient $r_L(m)$ and $\sigma=1/2$, bounds it by

$$
O\left(\log(2Y)\sum_{m\le Y}r_L(m)^2\right)\ll\log(2Y)\sum_{m\le Y}d(m)^2\ll Y\log^4(2Y)\ll T(\log T)^4.
$$

This uses only the given [divisor-square summatory bound](../../../../../../divisor-square-summatory-bound.md). For bounded $T$, the desired conclusions follow by boundedness on compact segments, so these estimates may be read for large $T$ with $Y\ge2$. We have proved **the requested diagonal-plus-error estimate**:

$$
\boxed{\int_0^T|\zeta(1/2+it)|^4\,dt\ll T\sum_{\substack{n_1,n_2,n_3,n_4\le\sqrt{T/(2\pi)}\\n_1n_2=n_3n_4}}\frac1{\sqrt{n_1n_2n_3n_4}}+T(\log T)^4.}
$$

The diagonal sum equals $\sum_{m\le Y}r_L(m)^2/m\le\sum_{m\le Y}d(m)^2/m$. If $D(x)=\sum_{m\le x}d(m)^2\ll x\log^3(2x)$, then [partial summation](../../../../../../abel-s-summation-formula.md) gives

$$
\sum_{m\le Y}\frac{d(m)^2}{m}=\frac{D(Y)}Y+\int_1^Y\frac{D(x)}{x^2}\,dx\ll\log^4(2Y).
$$

Consequently **the full fourth-moment bound** is

$$
\boxed{\int_0^T|\zeta(1/2+it)|^4\,dt\ll T(\log T)^4\qquad(T\ge2).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 124](../../../paper-124-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
