<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Cartesian tensor](../../../../../cartesian-tensor.md) law is $T'_{ik}=Q_{ia}Q_{kb}T_{ab}$. In every complete [tensor contraction](../../../../../tensor-contraction.md), summation over a transformed index contracts a pair of $Q$ factors to a [Kronecker delta](../../../../../kronecker-delta.md). In detail,

$$
\alpha'=Q_{ia}Q_{ib}T_{ab}=\delta_{ab}T_{ab}=\alpha,
$$



$$
\beta'=Q_{ia}Q_{kb}Q_{kc}Q_{id}T_{ab}T_{cd}=\delta_{bc}\delta_{ad}T_{ab}T_{cd}=T_{ab}T_{ba}=\beta,
$$



$$
\gamma'=Q_{ia}Q_{kb}Q_{kc}Q_{md}Q_{me}Q_{if}T_{ab}T_{cd}T_{ef}=\delta_{bc}\delta_{de}\delta_{af}T_{ab}T_{cd}T_{ef}=T_{ab}T_{bd}T_{da}=\gamma.
$$

Thus all three are invariant under [rotations](../../../../../rotation-mathematics.md). They are $\operatorname{tr}T$, $\operatorname{tr}(T^2)$ and $\operatorname{tr}(T^3)$. For a real [symmetric tensor](../../../../../symmetric-tensor.md), [orthogonal diagonalization](../../../../../orthogonal-diagonalization-of-a-real-symmetric-matrix.md) gives

$$
\alpha=\sum_i\lambda_i,\qquad\beta=\sum_i\lambda_i^2,\qquad\gamma=\sum_i\lambda_i^3.
$$

Expanding $\prod_i(\lambda-\lambda_i)$ and using [Newton's identities](../../../../../newton-s-identities.md) to recover the [characteristic polynomial from traces of powers](../../../../../characteristic-polynomial-from-traces-of-powers.md) yields

$$
\boxed{\lambda^3-\alpha\lambda^2+\frac{\alpha^2-\beta}{2}\lambda-\frac{\alpha^3-3\alpha\beta+2\gamma}{6}=0.}
$$

Comparison identifies $\boxed{c_2=-1,\qquad c_1=\tfrac12,\qquad c_0=-\tfrac16}$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
