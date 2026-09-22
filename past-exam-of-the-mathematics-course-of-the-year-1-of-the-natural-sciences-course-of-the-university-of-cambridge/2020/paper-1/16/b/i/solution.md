<h1 id="16/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $N$ count rotten pieces. Each item supplies an independent [Bernoulli trial](../../../../../../bernoulli-trial.md) with success [probability](../../../../../../probability.md) $p$, so $N$ has a [binomial distribution](../../../../../../binomial-distribution.md) with parameters $10,p$. There are $\binom{10}{n}$ choices of the rotten items, and each such choice has [probability](../../../../../../probability.md) $p^n(1-p)^{10-n}$. Hence

$$
\boxed{P(N=n)=\binom{10}{n}p^n(1-p)^{10-n},\qquad n=0,\ldots,10.}
$$

For $p=0$ or $p=1$, interpret this as the corresponding distribution concentrated at zero or ten; no ambiguous $0^0$ evaluation is needed.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [16](../../../16.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
