<h1 id="2/e/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $n\geq2$ and $1\leq k\leq n-1$, the [factorial](../../../../../../factorial.md) formula for a [binomial coefficient](../../../../../../binomial-coefficient-split.md) gives

$$
\begin{aligned}
\binom{n-1}k+\binom{n-1}{k-1}
&=\frac{(n-1)!(n-k)}{k!(n-k)!}
+\frac{(n-1)!k}{k!(n-k)!}\\
&=\frac{n!}{k!(n-k)!}=\binom nk.
\end{aligned}
$$

This proves [Pascal's identity](../../../../../../pascal-s-rule.md). The boundary cases $k=0,n$ follow for $n\geq1$ using the usual extension $\binom mj=0$ for $j<0$ or $j>m$. The recurrence itself requires $n\geq1$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [E](../../e.md)
3. [2](../../../2.md)
4. [Discrete mathematics, continuous mathematics and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2014](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
