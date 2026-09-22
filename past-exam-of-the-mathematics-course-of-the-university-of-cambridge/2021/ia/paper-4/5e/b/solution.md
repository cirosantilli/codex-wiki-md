<h1 id="5e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [binomial theorem](../../../../../../binomial-theorem.md) states

$$
(x+y)^n=\sum_{r=0}^n\binom nrx^ry^{n-r}.
$$

The required sum is the coefficient of $x^n$ in

$$
(1-x)^n(1+x)^n=(1-x^2)^n.
$$

There is no $x^n$ term when $n$ is [odd](../../../../../../odd-number.md). When $n$ is [even](../../../../../../even-number.md), the relevant term has exponent $2(n/2)=n$ and coefficient $(-1)^{n/2}\binom n{n/2}$. Hence

$$
\sum_{r=0}^n(-1)^r\binom nr^2
=\begin{cases}
0,&n\text{ odd},\\
(-1)^{n/2}\binom n{n/2},&n\text{ even}.
\end{cases}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
