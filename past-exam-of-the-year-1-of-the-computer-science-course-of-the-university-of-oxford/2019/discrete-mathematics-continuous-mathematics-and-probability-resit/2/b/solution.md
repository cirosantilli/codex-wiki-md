<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $E_i$ be the [set](../../../../../set-split.md) of [permutations](../../../../../permutation.md) fixing object $i$. If a specified collection of $k$ objects is fixed, the remaining $n-k$ objects can be arranged in $(n-k)!$ ways. There are $\binom nk$ such collections. Applying the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) to exclude all fixed objects gives

$$
d_n=\sum_{k=0}^n(-1)^k\binom nk(n-k)!=n!\sum_{k=0}^n\frac{(-1)^k}{k!}.
$$

For $n\geq1$, the terms $k=0$ and $k=1$ cancel. Thus the number of [derangements](../../../../../derangement-of-a-permutation.md) is **$\displaystyle d_n=\frac{n!}{2!}-\frac{n!}{3!}+\cdots+(-1)^n\frac{n!}{n!}$**, interpreting the remaining [sum](../../../../../sum.md) as empty when $n=1$. The full [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) formula also gives $d_0=1$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [Discrete mathematics, continuous mathematics, and probability resit](../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
4. [2019](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
