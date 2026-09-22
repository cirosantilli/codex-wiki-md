<h1 id="3/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Define the deterministic function $f(t)=\mathbb E[M_t^2]$. The independent increments from part (i) show that $f$ is increasing and that $M_t^2-f(t)$ is a [martingale](../../../../../../../martingale-split.md). Mean-square continuity follows from path continuity and the Gaussian laws, so $f$ is continuous.

The [Itô formula](../../../../../../../ito-s-lemma.md) also says that $M_t^2-[M]_t$ is a [local martingale](../../../../../../../local-martingale.md). Their difference $[M]_t-f(t)$ is therefore a continuous [finite-variation process](../../../../../../../finite-variation-process.md) that is also a local martingale. By the theorem that a [continuous finite-variation local martingale is constant](../../../../../../../continuous-finite-variation-local-martingale-is-constant.md), and because the difference starts at zero,

$$
[M]_t=f(t)
$$

for all $t\geq0$ almost surely.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [Paper 202](../../../../paper-202-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
