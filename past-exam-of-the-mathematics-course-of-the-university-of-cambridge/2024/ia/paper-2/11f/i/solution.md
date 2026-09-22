<h1 id="11f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $B_n$ count the $+1$ steps. Then

$$
B_n\sim\operatorname{Binomial}(n,p),
\qquad S_n=B_n-(n-B_n)=2B_n-n.
$$

Consequently

$$
\boxed{
\mathbb P(S_n=2k-n)
=\binom nkp^kq^{\,n-k},
\quad k=0,\ldots,n,
}
$$

and $S_n$ has probability zero at integers of the other parity. This is the finite-time law of a [simple random walk on the integer line](../../../../../../simple-random-walk-on-the-integer-line.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [11F](../../11f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ia](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
