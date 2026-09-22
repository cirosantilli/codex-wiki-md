<h1 id="21g/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

If $X$ is compact and $f:X\to\mathbb R$ is continuous, then $f(X)$ is compact by the [continuous image of a compact space](../../../../../../continuous-image-of-a-compact-space.md) theorem. Every compact subset of $\mathbb R$ is bounded, so $f$ is bounded.

Conversely, suppose the metric space $X$ is not compact. For metric spaces, compactness is equivalent to [sequential compactness](../../../../../../sequentially-compact-space.md), so there is a sequence of distinct points $(x_n)$ having no convergent subsequence. The set

$$
A=\{x_n:n\geq1\}
$$

is closed: an accumulation point would supply a convergent subsequence. It is also discrete for the same reason. Consequently the function

$$
g:A\to\mathbb R,
\qquad g(x_n)=n,
$$

is continuous. By part (a), $X$ is normal, and the [Tietze extension theorem](../../../../../../tietze-extension-theorem.md) extends $g$ to a continuous $G:X\to\mathbb R$. Since $G(x_n)=n$, this extension is unbounded. Therefore, if every continuous real-valued function on $X$ is bounded, $X$ must be compact. This is the [bounded-continuous-function characterization of compact metric spaces](../../../../../../bounded-continuous-function-characterization-of-compact-metric-spaces.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [21G](../../21g.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
