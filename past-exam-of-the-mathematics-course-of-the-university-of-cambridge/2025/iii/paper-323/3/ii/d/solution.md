<h1 id="3/ii/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Extend the [quantum conditional entropy](../../../../../../../quantum-conditional-entropy.md) from normalized states to positive operators by

$$
F(X_{AB})
=-\operatorname{Tr}(X_{AB}\log X_{AB})
+\operatorname{Tr}(X_B\log X_B).
$$

Since $\operatorname{Tr}X_{AB}=\operatorname{Tr}X_B$, the two terms involving $\log t$ cancel under $X\mapsto tX$, so $F(tX)=tF(X)$. Thus $F$ is [positively homogeneous](../../../../../../../positively-homogeneous-function-degree-one.md), and part (b) extends its [concavity](../../../../../../../concave-function.md) from states to the positive cone.

Apply part (c) with $X=\sigma_{AB}$ and $Y=\rho_{AB}$. Differentiating the [matrix logarithm](../../../../../../../matrix-logarithm.md) under the trace gives

$$
\left.\frac d{dt}\right|_{t=0}F(\sigma+t\rho)
=-\operatorname{Tr}(\rho\log\sigma)
+\operatorname{Tr}(\rho_B\log\sigma_B).
$$

The inequality from part (c), after moving $F(\rho)$ to the left, becomes

$$
\boxed{
D(\rho_{AB}\|\sigma_{AB})
\geq D(\rho_B\|\sigma_B)}.
$$

This is the [data-processing inequality for quantum relative entropy](../../../../../../../data-processing-inequality-for-quantum-relative-entropy.md) under [partial trace](../../../../../../../partial-trace.md). Tensoring each output with the appropriate maximally mixed state does not change either side, so it also proves data processing under normalized partial traces. Singular $\sigma$ follows by approximation on its support.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [Ii](../../ii.md)
3. [3](../../../3.md)
4. [Paper 323](../../../../paper-323-split.md)
5. [Iii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
