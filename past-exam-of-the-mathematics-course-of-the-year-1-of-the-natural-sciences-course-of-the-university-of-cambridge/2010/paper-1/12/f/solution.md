<h1 id="12/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

First take $1\leq n\leq F-1$. The forward object reaches $n$ at its $n$th move, while the reverse object reaches that label at its $(F-n)$th move. If the forward object wins after $k$ reverse moves, then $0\leq k\leq F-n-1$. The final choice is forward; among the preceding $n+k-1$ choices, exactly $k$ are reverse. By the [negative binomial stopping argument](../../../../../negative-binomial-stopping-argument.md), this case has [probability](../../../../../probability.md) $\binom{n-1+k}{k}p^nq^k$.

Sum these mutually exclusive cases and equate the result to part (e), using parts (b) and (d). This proves the [success-failure stopping identity](../../../../../success-failure-stopping-identity.md) here:

$$
\sum_{k=0}^{F-n-1}\binom{n-1+k}{k}p^nq^k
=\binom{F-1}{n}p^nq^{F-n}
+\sum_{k=n+1}^{F}\binom Fk p^kq^{F-k}.
$$

The right side splits the same race into a special meeting at $n$ and all meetings beyond $n$; the left side splits it according to the number of reverse moves at the winning time.

At $n=F$, both sides are zero with an [empty sum](../../../../../empty-sum.md) and $\binom{F-1}{F}=0$. At $n=0$, the event has [probability](../../../../../probability.md) one; the right side equals $\sum_{k=0}^{F}\binom Fk p^kq^{F-k}=1$. The printed left side includes $\binom{-1}{0}$ and is outside the usual nonnegative-upper-index combinatorial definition. With the explicit generalized convention **$\binom{-1}{0}=1$**, its $k=0$ term is one and all $k\geq1$ terms vanish, so the identity also holds at that endpoint. Without this convention the displayed sum is undefined there; the zero-target race must instead be stated separately. All identities extend to $p=0,1$ by their [polynomial](../../../../../polynomial-split.md) forms.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [12](../../12.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
