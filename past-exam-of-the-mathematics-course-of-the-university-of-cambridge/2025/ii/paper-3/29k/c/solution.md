<h1 id="29k/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Condition on the first risk-neutral move. After a factor $1+a$, homogeneity of the call payoff gives

$$
\left((1+a)S_N-K\right)^+
=(1+a)\left(S_N-\frac K{1+a}\right)^+,
$$

and the analogous identity holds for $1+b$. Therefore the [binomial call-price recursion](../../../../../../binomial-call-price-recursion.md) is

$$
\operatorname{EC}(N+1,K)
=u\,\operatorname{EC}\left(N,\frac K{1+a}\right)
+v\,\operatorname{EC}\left(N,\frac K{1+b}\right),
$$

with

$$
\boxed{
u=\frac{(1+a)(b-r)}{(1+r)(b-a)},
\qquad
v=\frac{(1+b)(r-a)}{(1+r)(b-a)}}.
$$

The inequalities $a<r<b$ and $a>-1$ make both coefficients positive.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [29K](../../29k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
