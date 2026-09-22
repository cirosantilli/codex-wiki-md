<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Write $S=\sin\theta_d$, $C=\cos\theta_d$. The chosen feedback parameters give $q=-C$ and $\alpha=SC/4$. Substitute the desired state directly into the dynamics, rather than dividing by a [determinant](../../../../../../determinant.md) that can vanish:

$$
\dot x\big|_{(S,C)}=-\tfrac12 C^2S+2(SC/4)C=0,
$$



$$
\dot z\big|_{(S,C)}=-2(SC/4)S-\tfrac12(C^2+1)C+C
=\tfrac C2(1-S^2-C^2)=0.
$$

Taking $y=0$ makes its derivative zero as well. Hence **the prescribed state is stationary for every target angle**, including the equator. It is pure because $S^2+C^2=1$ in this Pauli normalization.

For $C\ne0$, $D=C^2(C^2+1)+S^2C^2=2C^2$, and the expressions in (d) reduce to $x_*=S$, $z_*=C$, confirming uniqueness. For $C=0$, both $q$ and $\alpha$ vanish and $D=0$. The desired equatorial state is still stationary by direct substitution, but belongs to the whole stationary segment $(x,0)$; the singular formula cannot be used to claim unique stabilization.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 52](../../../paper-52-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
