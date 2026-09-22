<h1 id="2h/solution">Solution</h1>

↑ **Parent:** [2H](../2h.md)

Assume for contradiction that $\pi=a/b$ with positive [integers](../../../../../integer.md) $a,b$. Define

$$
F_n(x)=\frac{b^n}{n!}x^n(\pi-x)^n
=\frac1{n!}x^n(a-bx)^n
$$

and

$$
I_n=\int_0^\pi F_n(x)\sin x\,dx.
$$

The coefficient of $x^{n+j}$ in $F_n$ is

$$
\frac{(-1)^j}{n!}\binom nj a^{n-j}b^j.
$$

Consequently every derivative $F_n^{(k)}(0)$ is an integer: it is zero unless $n\leq k\leq2n$, and in that range the factor $k!/n!$ clears the denominator. Since $F_n(\pi-x)=F_n(x)$, every $F_n^{(k)}(\pi)$ is also an integer.

Repeated [integration by parts](../../../../../integration-by-parts.md), ending when derivatives above degree $2n$ vanish, gives

$$
I_n=\sum_{j=0}^n(-1)^j
\left(F_n^{(2j)}(0)+F_n^{(2j)}(\pi)\right).
$$

Thus $I_n$ is an integer. It is strictly positive because $F_n(x)\sin x>0$ for $0<x<\pi$.

On the other hand, $x(\pi-x)\leq\pi^2/4$, so

$$
0<I_n
\leq\frac{\pi}{n!}\left(\frac{b\pi^2}{4}\right)^n.
$$

The [factorial-over-power series](../../../../../factorial-over-power-series.md) implies that the right-hand side tends to zero. For all sufficiently large $n$ this says that the positive integer $I_n$ is less than one, a contradiction. Therefore the [Irrationality of pi](../../../../../proof-that-pi-is-irrational.md) is established:

$$
\boxed{\pi\notin\mathbb Q.}
$$

## ↑ Ancestors (10)

1. [2H](../2h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
