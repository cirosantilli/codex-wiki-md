<h1 id="8/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

Both sides of (ii) are [polynomials](../../../../../../polynomial-split.md) in the colour count, and they agree at every [integer](../../../../../../integer-split.md) $x\ge2$. A nonzero [polynomial](../../../../../../polynomial-split.md) has only finitely many roots, so this is a [polynomial identity](../../../../../../polynomial-identity.md) and holds also at $x=0,1$. It can therefore be evaluated at every possible value of the [Poisson random variable](../../../../../../poisson-distribution.md) $X$.

Take [expectations](../../../../../../expected-value-split.md) and use the [factorial moments](../../../../../../factorial-moment.md) from (a)(iv). The sum over $k$ is finite, so [linearity of expectation](../../../../../../linearity-of-expectation.md) gives

$$
\mathbb E[X^n]
=\sum_{k=1}^nA(n,k)\mathbb E[X(X-1)\cdots(X-k+1)]
=\sum_{k=1}^nA(n,k)=B(n).
$$

Combining this with (iii) proves [Dobiński's formula](../../../../../../dobinski-s-formula.md) for the [Bell numbers](../../../../../../bell-number.md):

$$
\boxed{B(n)=\frac1e\sum_{j=0}^{\infty}\frac{j^n}{j!}\qquad(n\ge1).}
$$

For completeness, the empty [set](../../../../../../set-split.md) has one [partition of a set](../../../../../../partition-of-a-set.md), giving $B(0)=1$; that case uses the empty-product conventions $0^0=1$ in this identity and a $k=0$ term in the partition sum.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability](../../../../discrete-mathematics-continuous-mathematics-and-probability-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
