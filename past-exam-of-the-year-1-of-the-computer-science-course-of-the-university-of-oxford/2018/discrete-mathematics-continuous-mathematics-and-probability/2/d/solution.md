<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Absorb the finitely many exceptional initial terms in the [Big O notation](../../../../../big-o-notation.md) assumption into a constant $C>0$, so that $|a_n|\leq Cn$ for every $n\geq1$. This is possible because each initial term is finite and each index is positive. We prove the stronger bound $|{}^kb_n|\leq Cn$ for every $k,n\geq1$.

The case $k=1$ is the chosen bound. If it holds at $k-1$, the [triangle inequality](../../../../../triangle-inequality.md) gives

$$
|{}^kb_n|\leq\frac1n\sum_{j=1}^n|{}^{k-1}b_j|\leq\frac Cn\sum_{j=1}^n j=\frac{C(n+1)}2\leq Cn.
$$

[Mathematical induction](../../../../../mathematical-induction.md) completes the proof. Thus **${}^kb_n=O(n)$ for every fixed $k$**; in fact the same constant works for all the iterated [Cesàro means](../../../../../cesaro-mean.md). This is the [linear-growth bound for iterated Cesàro means](../../../../../linear-growth-bound-for-iterated-cesaro-means.md).

## ↑ Ancestors (12)

1. [D](../d.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability](../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
4. [2018](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
