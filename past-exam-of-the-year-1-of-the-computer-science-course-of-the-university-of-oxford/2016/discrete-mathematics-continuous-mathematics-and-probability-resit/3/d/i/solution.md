<h1 id="3/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use [natural logarithms](../../../../../../natural-logarithm.md); the same argument works for any fixed base greater than $1$. The [function](../../../../../../function-split.md) $\log\log x$ is increasing for $x>1$, since its [derivative](../../../../../../derivative.md) is $1/(x\log x)>0$. With natural logs the sole negative summand is at $i=2$. Put $C_0=|\log\log2|$.

For all sufficiently large $n$ with $\log\log n\geq1$, monotonicity and the [triangle inequality](../../../../../../triangle-inequality.md) give

$$
\left|\sum_{i=2}^n\log\log i\right|
\leq C_0+\sum_{i=3}^n\log\log i
\leq C_0+n\log\log n
\leq(1+C_0)n\log\log n.
$$

These are fixed constants and an eventual bound, proving

$$
\boxed{\sum_{i=2}^n\log\log i=O(n\log\log n)}.
$$

For another fixed logarithm base there are still only finitely many negative initial terms, which are absorbed in $C_0$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [3](../../../3.md)
4. [Discrete mathematics, continuous mathematics and probability (resit)](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2016](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
