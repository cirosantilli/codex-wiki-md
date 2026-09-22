<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

This is a normalized [perceptron algorithm](../../../../../../perceptron.md). Because $\|Z_i\|_2=1$, an update on a misclassified point obeys

$$
\begin{aligned}
\|\gamma^{(m+1)}-\widehat\gamma\|_2^2
&=\|\gamma^{(m)}-\widehat\gamma+Y_iZ_i\|_2^2\\
&=\|\gamma^{(m)}-\widehat\gamma\|_2^2+1
+2Y_iZ_i^T\gamma^{(m)}-2Y_iZ_i^T\widehat\gamma\\
&\leq\|\gamma^{(m)}-\widehat\gamma\|_2^2+1+0-2\\
&=\|\gamma^{(m)}-\widehat\gamma\|_2^2-1.
\end{aligned}
$$

Here the two inequalities use the update condition $Y_iZ_i^T\gamma^{(m)}\leq0$ and the assumed unit margin $Y_iZ_i^T\widehat\gamma\geq1$. A squared distance cannot become negative, so there can be at most $\|\gamma^{(0)}-\widehat\gamma\|_2^2$ updates. The algorithm then returns a vector that correctly separates every training point. The estimate $\widehat\gamma$ is the comparison vector for the proof; without an additional uniqueness condition the returned separator need not equal that particular vector.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
