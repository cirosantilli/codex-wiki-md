<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let

$$
\delta(u)=\mathbb E[A\mid Z=1,U=u]
-\mathbb E[A\mid Z=0,U=u]
$$

and

$$
\tau(u)=\mathbb E[Y(1)-Y(0)\mid U=u].
$$

Because $U$ contains all exposure-outcome confounding and $Z$ is independent of $U$, the exclusion restriction and the law of total expectation give

$$
\mathbb E[Y\mid Z=1]-\mathbb E[Y\mid Z=0]
=\mathbb E\{\tau(U)\delta(U)\}.
$$

Likewise,

$$
\mathbb E[A\mid Z=1]-\mathbb E[A\mid Z=0]
=\mathbb E\{\delta(U)\}.
$$

The no [confounder-instrument interaction](../../../../../../confounder-instrument-interaction.md) assumption says $\delta(U)=\delta$ is constant. Relevance gives $\delta\ne0$, so the Wald ratio is

$$
\frac{\delta\,\mathbb E\tau(U)}{\delta}
=\mathbb E[Y(1)-Y(0)],
$$

the overall [average treatment effect](../../../../../../average-treatment-effect.md).

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 221](../../../paper-221-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
