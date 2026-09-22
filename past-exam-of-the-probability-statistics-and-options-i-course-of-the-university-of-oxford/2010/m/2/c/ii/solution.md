<h1 id="m/2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Starting at one, state two can first be reached only after an even number of steps. At every even time before that hit, the chain is again at one. By the [Markov property](../../../../../../markov-property.md) and part (i), each successive two-step block hits two with [probability](../../../../../../probability.md) $4/9$, while a failure returns to one with [probability](../../../../../../probability.md) $5/9$. Therefore, for the first hitting time $H$,

$$
\boxed{\mathbb P(H=2k)=\left(\frac59\right)^{k-1}\frac49\quad(k\geq1),\qquad\mathbb P(H\text{ odd})=0.}
$$

Equivalently $H/2$ has the [geometric distribution](../../../../../../geometric-distribution.md) on the positive integers with success [probability](../../../../../../probability.md) $4/9$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [M](../../../../m.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../../../split.md)
7. [Probability, statistics and options I course of the University of Oxford](../../../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
9. [Mathematics and statistics course of the University of Oxford](../../../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
