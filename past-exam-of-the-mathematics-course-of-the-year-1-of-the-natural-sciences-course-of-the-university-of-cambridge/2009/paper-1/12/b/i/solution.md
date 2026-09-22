<h1 id="12/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For the last chocolate to be taken on choice $n$, the first $n-1$ choices must include exactly $C-1$ chocolate choices, and choice $n$ must take chocolate. Before that final success there is still chocolate available, so no forced plain choice has yet occurred. The [negative binomial stopping argument](../../../../../../negative-binomial-stopping-argument.md) gives

$$
\boxed{P_{\rm LastChoc,n}=\binom{n-1}{C-1}p^C(1-p)^{n-C},\qquad C\leq n\leq F.}
$$

This is the all-trials convention of the [negative binomial distribution](../../../../../../negative-binomial-distribution.md). The finite examination scenario also has a remaining probability that the tray still contains chocolate after all $F$ choices; the displayed probabilities need not sum to one over $C\leq n\leq F$. At $p=0$ the last chocolate is never taken, and at $p=1$ it is taken on choice $C$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [12](../../../12.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
