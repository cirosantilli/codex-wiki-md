<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The sequence of norms is bounded. Choose $M>\sup_n\|x_n\|$ and $M>\|x\|$. By the [spectral radius formula](../../../../../../spectral-radius-formula.md), every relevant spectrum lies in $|\lambda|<M$. The compact set $K=\{\lambda:|\lambda|\leq M\}\setminus U$ is disjoint from $\sigma(x)$. If nonempty, continuity of the [resolvent of an element](../../../../../../resolvent-of-an-element.md) gives $C=\sup_K\|(\lambda1-x)^{-1}\|<\infty$. For large $n$, $C\|x_n-x\|<1$, and

$$
\lambda1-x_n=(\lambda1-x)\left[1-(\lambda1-x)^{-1}(x_n-x)\right]
$$

is invertible for every $\lambda\in K$ by the [Neumann series](../../../../../../neumann-series.md). If $K$ is empty there is nothing to exclude. No spectral points can lie outside the radius-$M$ disc either. Consequently **$\sigma(x_n)\subset U$ for all sufficiently large $n$**. Taking $U$ to be the disc of radius $r(x)+\varepsilon$ also proves upper semicontinuity of the [spectral radius](../../../../../../spectral-radius.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 10](../../../paper-10-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
