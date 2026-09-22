<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Optimality gives $Q(\widehat\beta)\leq Q(\beta^0)$. Substitute $Y=X\beta^0+\varepsilon$, expand both squared norms, and cancel $\lVert\varepsilon\rVert_2^2/(2n)$. Rearranging gives

$$
\frac1{2n}\lVert X(\beta^0-\widehat\beta)\rVert_2^2
\leq\frac1n\varepsilon^TX(\widehat\beta-\beta^0)
+\lambda(\lVert\beta^0\rVert_1-\lVert\widehat\beta\rVert_1).
$$

This exposes a factor-of-two typo in the paper: its requested display has $1/n$ rather than $1/(2n)$ on the left while leaving the right side unchanged. For the objective printed in the paper, the displayed inequality above is the correct basic inequality. Part (b) explicitly asks us to use the stronger stated version, so the subsequent argument proceeds from that requested premise.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
