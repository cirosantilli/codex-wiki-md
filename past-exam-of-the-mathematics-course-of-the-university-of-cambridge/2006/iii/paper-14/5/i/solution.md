<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $S$ be the number of red vertices in $W$. It has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $r$ and $1/2$, so [independence](../../../../../../independent-random-variables.md) gives

$$
\mathbb E e^{t(S-r/2)}=\left(\cosh(t/2)\right)^r.
$$

For $t=1$, the strict inequality $\log\cosh(1/2)<1/8$ follows by integrating $\tanh u<u$ for $u>0$. Hence the [exponential Markov bound](../../../../../../exponential-markov-bound.md) yields

$$
\mathbb P(S>3r/4)
\leq e^{-r/4}\left(\cosh(1/2)\right)^r
<e^{-r/4+r/8}.
$$

Therefore

$$
\boxed{\mathbb P(S>3r/4)<e^{-r/8}.}
$$

This supplies the tail estimate directly, including the strict constant in the requested bound.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 14](../../../paper-14-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
