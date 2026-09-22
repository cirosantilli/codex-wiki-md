<h1 id="13j/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Because $I-H$ is an orthogonal projection of rank $n-p$,

$$
\begin{aligned}
\mathbb E\|Y-HY\|^2
&=\mathbb E\|(I-H)(\mu+\varepsilon)\|^2\\
&=\|(I-H)\mu\|^2
 +\sigma^2\operatorname{tr}(I-H)\\
&=\|(I-H)\mu\|^2+(n-p)\sigma^2.
\end{aligned}
$$

It follows that [Mallows Cp](../../../../../../mallows-s-cp.md) satisfies

$$
\begin{aligned}
\mathbb E[C_p]
&=\mathbb E\|Y-HY\|^2+2p\sigma^2\\
&=\|(I-H)\mu\|^2+(n+p)\sigma^2\\
&=\mathbb E\|HY-Y^*\|^2,
\end{aligned}
$$

where the last equality is part (i). Thus $C_p$ is an [unbiased estimator](../../../../../../unbiased-estimator.md) of the independent-copy prediction error, as summarized by the [unbiased prediction-error identity for ordinary least squares](../../../../../../unbiased-prediction-error-identity-for-ordinary-least-squares.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [13J](../../13j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
