<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

On $[\tau,\sigma)$ the Brownian path does not meet zero, so the [power function](../../../../../../power-function-of-a-statistical-test.md) $x\mapsto|x|^\delta$ is twice continuously differentiable along the path. The [Itô formula](../../../../../../ito-s-lemma.md) gives

$$
dY_t=\delta|B_t|^{\delta-1}\operatorname{sign}(B_t)dB_t+\frac{\delta(\delta-1)}2|B_t|^{\delta-2}dt.
$$

Since $Y_t=|B_t|^\delta$, this becomes

$$
dY_t=\delta Y_t^{(\delta-1)/\delta}d\widehat B_t+\frac{\delta(\delta-1)}2Y_t^{(\delta-2)/\delta}dt,
$$

where $\widehat B_t=\int_0^t\operatorname{sign}(B_s)dB_s$ is a standard [Brownian motion](../../../../../../brownian-motion-split.md) by the [Lévy characterization of Brownian motion](../../../../../../levy-characterization-of-brownian-motion.md). Thus the displayed equation in the paper is valid after the customary renaming of $\widehat B$ as $B$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
