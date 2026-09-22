<h1 id="1/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

Use two results: the isometric [Stinespring dilation](../../../../../../stinespring-dilation.md) of a [quantum channel](../../../../../../quantum-channel.md), and [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md). Let $V:B\to B'E$ dilate the given operation, and define

$$
\omega_{AB'E}=(I_A\otimes V)\rho_{AB}(I_A\otimes V^\dagger),\qquad\sigma_{AB'}=\operatorname{Tr}_E\omega.
$$

An [linear isometry of Hilbert spaces](../../../../../../linear-isometry-of-hilbert-spaces.md) preserves the nonzero [eigenvalues](../../../../../../eigenvalue.md), so $S(B'E)_\omega=S(B)_\rho$ and $S(AB'E)_\omega=S(AB)_\rho$. Subtracting the two [coherent information](../../../../../../coherent-information.md) expressions gives

$$
\begin{aligned}
I(A\rangle B)_\rho-I(A\rangle B')_\sigma
&=S(B'E)_\omega-S(AB'E)_\omega-S(B')_\omega+S(AB')_\omega\\
&=I(A:E|B')_\omega\geq0.
\end{aligned}
$$

The last inequality is [Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md), in the form $S(AB')+S(B'E)\geq S(B')+S(AB'E)$. Thus the [data-processing inequality for coherent information](../../../../../../data-processing-inequality-for-coherent-information.md) is

$$
\boxed{I(A\rangle B)_\rho\geq I(A\rangle B')_\sigma.}
$$

The lost [coherent information](../../../../../../coherent-information.md) is precisely the [quantum conditional mutual information](../../../../../../quantum-conditional-mutual-information.md) between the reference $A$ and discarded environment $E$, conditional on the retained output $B'$.

## ↑ Ancestors (11)

1. [V](../v.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
