<h1 id="4/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

On the panel $[2j/n,2(j+1)/n]$, the maximum fourth [derivative](../../../../../../derivative.md) is at the left endpoint because it is decreasing. Thus

$$
E_n\le\frac1{90n^5}\sum_{j=0}^{n/2-1}
\left(e^{2j/n}-\frac{2ej}{n}\right).
$$

The [geometric series](../../../../../../geometric-series.md) and the sum of consecutive integers give

$$
\sum_{j=0}^{n/2-1}e^{2j/n}=\frac{e-1}{e^{2/n}-1},\qquad
\frac{2e}{n}\sum_{j=0}^{n/2-1}j=\frac{en}{4}-\frac e2.
$$

Substitution proves

$$
\boxed{E_n\le B(n):=\frac1{90n^5}
\left(\frac{e-1}{e^{2/n}-1}-\frac{en}{4}+\frac e2\right).}
$$

For $n>2$, at least one panel's maximum is smaller than the global maximum $1$, so this bound is strictly tighter than the global bound. For $n=2$, the two bounds coincide.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [4](../../../4.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
