<h1 id="a/2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For events $E_n$, the [Borel-Cantelli first lemma](../../../../../borel-cantelli-first-lemma.md) states that $\sum_n\mathbb P(E_n)<\infty$ implies $\mathbb P(E_n\text{ infinitely often})=0$. Indeed,

$$
\mathbb P\left(\bigcup_{n\geq m}E_n\right)\leq\sum_{n\geq m}\mathbb P(E_n)\to0.
$$

These unions decrease to $\limsup E_n$, so continuity from above proves the assertion.

The [Borel-Cantelli second lemma](../../../../../borel-cantelli-second-lemma.md) states that independent events with $\sum_n\mathbb P(E_n)=\infty$ satisfy $\mathbb P(E_n\text{ infinitely often})=1$. For every fixed $m$, independence and $1-x\leq e^{-x}$ give

$$
\mathbb P\left(\bigcap_{n=m}^N E_n^c\right)=\prod_{n=m}^N(1-\mathbb P(E_n))
\leq\exp\left(-\sum_{n=m}^N\mathbb P(E_n)\right)\to0.
$$

Continuity from above shows there is probability zero of no event after $m$. A countable union over $m$ gives probability zero of only finitely many occurrences. Independence is needed for this second conclusion, but not for the first.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
