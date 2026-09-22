<h1 id="3/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Because the two flags $E_C$ and $F_C$ are [orthogonal projections](../../../../../../../orthogonal-projection.md), the flagged state is block diagonal. If $h(\lambda)$ denotes the [binary entropy](../../../../../../../binary-entropy.md), then

$$
S(\rho_{ABC})
=h(\lambda)+\lambda S(\rho'_{AB})
+(1-\lambda)S(\rho''_{AB}),
$$

and

$$
S(\rho_{BC})
=h(\lambda)+\lambda S(\rho'_B)
+(1-\lambda)S(\rho''_B).
$$

Its unflagged marginals are $\rho_{AB}=\lambda\rho'_{AB}+(1-\lambda)\rho''_{AB}$ and $\rho_B=\lambda\rho'_B+(1-\lambda)\rho''_B$. Substitution in [Strong subadditivity of Von Neumann entropy](../../../../../../../strong-subadditivity-of-quantum-entropy.md) cancels the two binary-entropy terms and gives

$$
\boxed{
H(A|B)_{\lambda\rho'+(1-\lambda)\rho''}
\geq
\lambda H(A|B)_{\rho'}
+(1-\lambda)H(A|B)_{\rho''}}.
$$

This is exactly the [concavity of quantum conditional entropy](../../../../../../../concavity-of-quantum-conditional-entropy.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
