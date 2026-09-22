<h1 id="6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The two colonies with no observed cheaters are [right-censored](../../../../../right-censoring.md) after seven days. Each contributes $\Pr(X>7)=(1-p)^7$, not the [probability](../../../../../probability.md) of an event on day seven or eight. The four observed first events contribute four factors of $p$ and $(6-1)+(7-1)+(5-1)+(5-1)=19$ failures. Including the two censored exposures gives

$$
\mathcal L(p)\propto p^4(1-p)^{19+7+7}=p^4(1-p)^{33}.
$$

The [beta distribution](../../../../../beta-distribution.md) prior therefore yields

$$
\boxed{p\mid D\sim\operatorname{Beta}(9,38)},\qquad
\mathbb E[p\mid D]=\frac9{47}\simeq0.19149.
$$

Its [probability density function](../../../../../probability-density-function.md) is proportional to $p^8(1-p)^{37}$ for $0<p<1$: it vanishes at both endpoints, is unimodal, and has its [mode](../../../../../mode-statistics.md) at $8/45\simeq0.17778$. The right panel of the sketch in question 5(b) shows this moderately right-skewed density. The calculation assumes daily observations detect the first event and that stopping the experiment after seven days is [independent censoring](../../../../../independent-censoring.md).

## ↑ Ancestors (13)

1. [E](../e.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
