<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Fix $m\geq0$, using the convention for [binomial coefficients](../../../../../binomial-coefficient-split.md) that $\binom{k}{m}=0$ when $m>k$. At $n=0$, both $\binom0m$ and $\binom1{m+1}$ equal $1$ if $m=0$ and $0$ otherwise.

For the successor step, apply the [induction hypothesis](../../../../../induction-hypothesis.md), then [Pascal's rule](../../../../../pascal-s-rule.md):

$$
\sum_{k=0}^{n+1}\binom{k}{m}
=\binom{n+1}{m+1}+\binom{n+1}{m}
=\binom{n+2}{m+1}.
$$

Thus [mathematical induction](../../../../../mathematical-induction.md) proves the [hockey-stick identity](../../../../../hockey-stick-identity.md)

$$
\boxed{\sum_{k=0}^{n}\binom{k}{m}=\binom{n+1}{m+1}\quad(m,n\geq0)}.
$$

The zero convention also covers the case $n<m$, without a separate starting index.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics and probability (resit)](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
