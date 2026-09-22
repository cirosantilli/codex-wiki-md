<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each rotation, [unitarity](../../../../../../unitary-operator.md) gives

$$
 \|U_{ij,\theta}F-F\|_2^2
 =2\|F\|_2^2-2\operatorname{Re}\langle F,U_{ij,\theta}F\rangle.
$$

Averaging and using self-adjointness of $Q$ yields the [Dirichlet form of the Kac collision operator](../../../../../../dirichlet-form-of-the-kac-collision-operator.md)

$$
 \boxed{\langle F,(I-Q)F\rangle
 =\frac1{4\pi C_N}\sum_{i<j}\int_0^{2\pi}\int_{\mathbb R^N}
 |F(R_{ij,\theta}\mathbf v)-F(\mathbf v)|^2\,d\mathbf v\,d\theta.}
$$

The velocity [integral](../../../../../../integral.md) is necessary: its omission from the printed right-hand side would leave a function of $\mathbf v$ rather than a scalar. This identity applies to every $L^2$ function, with complex modulus when necessary, and is nonnegative.

If $(I-Q)F=0$, every nonnegative angular [integral](../../../../../../integral.md) is zero, so $\|U_{ij,\theta}F-F\|_2=0$ for almost every angle. Strong continuity in angle extends equality to every angle. The coordinate-plane [Givens rotations](../../../../../../givens-rotation.md) generate the [special orthogonal group](../../../../../../special-orthogonal-group.md) $SO(N)$, hence $F$ is invariant in $L^2$ under every element of this group. To identify its shape rigorously despite almost-everywhere representatives, average over the normalized [Haar measure](../../../../../../haar-measure.md) of $SO(N)$. This averaging leaves $F$ unchanged, while transitivity of the rotation group on each sphere makes the average a [radial function](../../../../../../radial-function.md). Thus $F(\mathbf v)=\phi(|\mathbf v|)$ almost everywhere.

Conversely, every [radial function](../../../../../../radial-function.md) is fixed by every coordinate-plane rotation, and so by $Q$. Therefore

$$
 \boxed{\ker(I-Q)=\{F\in L^2(\mathbb R^N):F(\mathbf v)=\phi(|\mathbf v|)\ \text{a.e.}\}.}
$$

This is the [radial kernel of the Kac collision operator](../../../../../../radial-kernel-of-the-kac-collision-operator.md). The rotation correction is essential to this conclusion: with the literal printed map, even $F(\mathbf v)=e^{-|\mathbf v|^2}$ in dimension two is not fixed. At $\mathbf v=(0,1)$ its printed-map angular average is the average of $e^{-\sin^2\theta}$, strictly greater than its value $e^{-1}$.

## ↑ Ancestors (11)

1. [B](../b.md)
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
