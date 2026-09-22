<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use base-two logarithms, so the [Von Neumann entropy](../../../../../../von-neumann-entropy-split.md) is $S(\rho)=-\operatorname{Tr}(\rho\log_2\rho)$, with $0\log0=0$. The [quantum mutual information](../../../../../../quantum-mutual-information.md) is $I(A:B)=S(A)+S(B)-S(AB)$; this is the quantity denoted by $S(\rho_A:\rho_B)$ in the question, using the given joint state.

[Strong subadditivity of Von Neumann entropy](../../../../../../strong-subadditivity-of-quantum-entropy.md) states that for every tripartite [density operator](../../../../../../density-matrix.md),

$$
\boxed{S(AB)+S(BC)\ge S(B)+S(ABC).}
$$

Equivalently the conditional [quantum mutual information](../../../../../../quantum-mutual-information.md) $I(A:C\mid B)$ is nonnegative. We apply this property to the original state or to a dilation of the relevant [quantum channel](../../../../../../quantum-channel.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
