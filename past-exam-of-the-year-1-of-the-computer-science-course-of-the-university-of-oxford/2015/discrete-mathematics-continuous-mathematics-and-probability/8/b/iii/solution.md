<h1 id="8/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Using the [probability mass function](../../../../../../probability-mass-function.md) of the [Poisson distribution](../../../../../../poisson-distribution.md) directly gives

$$
\boxed{\mathbb E[X^n]=\frac1e\sum_{j=0}^{\infty}\frac{j^n}{j!}.}
$$

For each fixed positive [integer](../../../../../../integer-split.md) $n$, this [series](../../../../../../series-mathematics.md) converges: the [ratio](../../../../../../ratio.md) of successive nonzero terms is $(1+1/j)^n/(j+1)$, which tends to zero. Equivalently, using the [polynomial identity](../../../../../../polynomial-identity.md) in (ii) and the [factorial moments](../../../../../../factorial-moment.md) from (a)(iv) gives $\mathbb E[X^n]=\sum_{k=1}^nA(n,k)$; the extension of that identity to $X=0,1$ is justified in (iv).

## ↑ Ancestors (13)

1. [Iii](../iii.md)
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
