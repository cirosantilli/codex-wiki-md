<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the genuine planar [Givens rotation](../../../../../../givens-rotation.md)

$$
 \binom{v_i(\theta)}{v_j(\theta)}
 =\begin{pmatrix}\cos\theta&\sin\theta\\-\sin\theta&\cos\theta\end{pmatrix}
 \binom{v_i}{v_j}.
$$

In the second component the cosine multiplies $v_j$: the repeated $v_i$ in the printed formula is an error. With that printed expression, at $\theta=0$ the pair becomes $(v_i,v_i)$, which does not preserve length or measure. The rotation-based claims require the corrected expression. Also take $N\geq2$, since the normalization by $\binom N2$ is undefined for $N=1$.

Let $C_N=\binom N2$ and $U_{ij,\theta}F=F\circ R_{ij,\theta}$. The [change of variables formula](../../../../../../change-of-variables-formula.md) and determinant one give $\|U_{ij,\theta}F\|_2=\|F\|_2$. Thus each is a [unitary operator](../../../../../../unitary-operator.md), with adjoint $U_{ij,-\theta}$. The [Kac collision operator](../../../../../../kac-collision-operator.md) is the average

$$
 Q=\frac1{C_N}\sum_{i<j}\frac1{2\pi}\int_0^{2\pi}U_{ij,\theta}\,d\theta.
$$

The [Minkowski integral inequality](../../../../../../minkowski-integral-inequality.md) gives $\|QF\|_2\leq\|F\|_2$, so $Q$ is bounded. For the [Hilbert space](../../../../../../hilbert-space-split.md) [inner product](../../../../../../inner-product.md), integration and the angular change $\theta\mapsto-\theta$ give

$$
 \langle G,QF\rangle
 =\frac1{2\pi C_N}\sum_{i<j}\int_0^{2\pi}\langle U_{ij,-\theta}G,F\rangle d\theta
 =\langle QG,F\rangle.
$$

Hence **$Q=Q^*$ and $\|Q\|\leq1$**. In fact a nonzero radial [Gaussian function](../../../../../../gaussian-function.md) is fixed by every rotation, showing $\|Q\|=1$. Angular averages can be understood as strong [Bochner integrals](../../../../../../bochner-integral.md); continuity of rotations in $L^2$ follows first for smooth compactly supported functions, then by density.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
