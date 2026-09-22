<h1 id="2/d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the intended assumption that the two white-noise sequences are mutually uncorrelated at every pair of times, $X$ and $W$ are uncorrelated. Their sum is therefore weakly stationary with

$$
\mathbb EY_t=0,
\qquad
\gamma_Y(h)=
\frac{\sigma^2}{1-\phi^2}\phi^{|h|}
+\sigma_W^2\mathbf1_{\{h=0\}}.
$$

Strictly, the printed condition $\mathbb E[\varepsilon_tW_t]=0$ only at equal times is insufficient. For example, $W_t=(-1)^t\varepsilon_{t-1}$ is itself white noise and is contemporaneously uncorrelated with $\varepsilon_t$, but the cross-covariance contribution can depend on $t$. The displayed answer therefore uses the standard intended cross-series white-noise assumption $\mathbb E[\varepsilon_tW_s]=0$ for all $s,t$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [D](../../d.md)
3. [2](../../../2.md)
4. [Paper 218](../../../../paper-218-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
