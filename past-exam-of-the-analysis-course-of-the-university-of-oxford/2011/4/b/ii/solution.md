<h1 id="4/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For each fixed $n$, the coefficient functional is bounded since

$$
|\widehat f(n)|\leq\frac1{\sqrt{2\pi}}\int_{-\pi}^{\pi}|f(t)|\,dt
\leq\sqrt{2\pi}\|f\|_\infty.
$$

Suppose $f_j\to f$ and $Tf_j\to g$ uniformly. Taking coefficients and passing to the limit gives

$$
\widehat g(n)=\lim_j\widehat{Tf_j}(n)
=\alpha_n\lim_j\widehat f_j(n)=\alpha_n\widehat f(n)
$$

for every fixed $n$. No uniform bound on $\alpha_n$ is needed for this passage. Uniqueness gives $g=Tf$, so $T$ has a closed graph. The space $X$ is Banach, being the closed subspace defined by $f(-\pi)=f(\pi)$ inside the [continuous functions](../../../../../continuous-function.md) with the uniform [norm](../../../../../norm.md). The [closed graph theorem](../../../../../closed-graph-theorem.md) therefore proves **$T$ is bounded**.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the analysis course of the University of Oxford](../../../../split.md)
6. [Analysis course of the University of Oxford](../../../../../analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
