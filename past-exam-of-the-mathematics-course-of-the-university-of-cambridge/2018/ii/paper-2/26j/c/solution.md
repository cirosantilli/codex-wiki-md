<h1 id="26j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

From [convergence in probability](../../../../../../convergence-in-probability.md), choose a subsequence $X_{n_k}\to X$ almost surely. The [Fatou lemma](../../../../../../fatou-s-lemma.md) then gives

$$
\mathbb E|X|^2
\leq\liminf_{k\to\infty}\mathbb E|X_{n_k}|^2
\leq1,
$$

so $X\in L^2$.

The bounded second moments make $(X_n)$ [uniformly integrable](../../../../../../uniform-integrability-from-bounded-second-moments.md), and $X$ is integrable. Convergence in probability together with [uniform integrability](../../../../../../uniform-integrability.md) therefore gives

$$
\boxed{X_n\longrightarrow X\quad\text{in }L^1.}
$$

Convergence in $L^2$ need not follow. On $[0,1]$ with Lebesgue measure, let

$$
X_n=\sqrt n\,\mathbf1_{(0,1/n)},
\qquad X=0.
$$

Then $X_n\to0$ in probability and $\mathbb E|X_n|^2=1$, but $\lVert X_n\rVert_2=1$ for every $n$. This is the [bounded second moments do not upgrade convergence in probability to convergence in L2](../../../../../../bounded-second-moments-do-not-upgrade-convergence-in-probability-to-convergence-in-l2.md) example.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [26J](../../26j.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
