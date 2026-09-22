<h1 id="12g/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $g=1/f$. The hypothesis $|f(z)|\to\infty$ gives $g(z)\to0$ as $z\to a$, so defining $g(a)=0$ makes $g$ continuous on $U$ and analytic there by the stated assumption. Its zero at $a$ has some finite order $m\geq1$, and hence

$$
g(z)=(z-a)^m q(z),
\qquad q(a)\ne0.
$$

Therefore

$$
f(z)=(z-a)^{-m}\frac1{q(z)}
$$

has a pole of order $m$: its Laurent series has $c_{-m}\ne0$ and $c_n=0$ for $n<-m$.

Now let $f$ be entire and tend to infinity at infinity. The function

$$
h(z)=f(1/z)
$$

tends to infinity as $z\to0$, so the preceding argument says that $h$ has a pole at zero. If the [Taylor series](../../../../../../taylor-series.md) of $f$ is $f(w)=\sum_{n\geq0}a_nw^n$, then

$$
h(z)=\sum_{n\geq0}a_nz^{-n}.
$$

A pole has only finitely many negative powers, so $a_n=0$ for all sufficiently large $n$. Thus $f$ is a [polynomial](../../../../../../polynomial-split.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [12G](../../12g.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
