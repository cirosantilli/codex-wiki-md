<h1 id="22g/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Suppose the [spectrum](../../../../../../spectrum-functional-analysis.md) were empty. The resolvent

$$
R(\lambda)=(\lambda I-T)^{-1}
$$

would then be an entire operator-valued [function](../../../../../../function-split.md). For $|\lambda|>\|T\|$,

$$
R(\lambda)=\frac1\lambda\sum_{n=0}^\infty\left(\frac T\lambda\right)^n,
$$

because the [series](../../../../../../series-mathematics.md) converges in operator norm and multiplication by $\lambda I-T$ telescopes to $I$. Hence $\|R(\lambda)\|\leq(|\lambda|-\|T\|)^{-1}$.

For fixed $x,y\in\ell^2$, the [scalar](../../../../../../scalar.md) [function](../../../../../../function-split.md) $\langle R(\lambda)x,y\rangle$ is entire, bounded outside a disc by the estimate and bounded inside by compactness. Liouville's theorem makes it constant, and its [limit](../../../../../../limit-of-a-function.md) at infinity makes that constant zero. This for all $x,y$ would imply $R(\lambda)=0$, impossible for an inverse. Thus the [spectrum](../../../../../../spectrum-functional-analysis.md) is nonempty.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [22G](../../22g.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
