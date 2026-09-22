<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Part (d) makes the residual and therefore $\widehat\nu=X^T(Y-X\widehat\beta)$ unique, so $E$ is unique. The [Karush-Kuhn-Tucker conditions](../../../../../../karush-kuhn-tucker-conditions.md) from part (c) imply that every nonzero block satisfies $\lVert\widehat\nu^{(k)}\rVert_2=n\lambda\sqrt m$. Hence $\widehat\beta^{(k)}=0$ for $k\notin E$.

Any two minimizers have the same fitted value and vanish outside $E$. Their difference $h$ is therefore supported on $E$ and satisfies $\widetilde Xh_E=0$. If $\widetilde X$ has full column rank, then $h_E=0$, proving uniqueness of $\widehat\beta$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 205](../../../paper-205-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
