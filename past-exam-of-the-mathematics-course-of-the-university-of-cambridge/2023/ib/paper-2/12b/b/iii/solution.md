<h1 id="12b/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Write $h(z)=\sum_{n=0}^{\infty}a_nz^n$. Cauchy's coefficient formula on $|z|=R$ gives

$$
a_n=\frac1{2\pi R^n}
\int_0^{2\pi}h(Re^{i\theta})e^{-in\theta}\,d\theta.
$$

Except at the two measure-zero points where $\cos\theta=0$, the hypothesis gives

$$
|h(Re^{i\theta})|
\leq R^{-1/2}|\cos\theta|^{-1/2}.
$$

Since $|\cos\theta|^{-1/2}$ is integrable,

$$
|a_n|
\leq C R^{-n-1/2}
$$

for a constant $C$ independent of $R$. Letting $R\to\infty$ shows that every $a_n=0$. Hence $h\equiv0$, in particular $h$ is constant. This proves the [entire function under a horizontal inverse-square-root bound](../../../../../../../entire-function-under-a-horizontal-inverse-square-root-bound.md) result.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [12B](../../../12b.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
