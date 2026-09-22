<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $\Pi_G$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto $G$. The two [reflection operators](../../../../../../reflection-operator.md) are

$$
I_{|\psi\rangle}=I-2|\psi\rangle\langle\psi|,
\qquad
I_G=I-2\Pi_G.
$$

The first fixes the hyperplane $|\psi\rangle^\perp$ and changes the sign of $|\psi\rangle$; the second fixes $G^\perp$ and changes the sign of $G$.

Write the normalized projections of $|\psi\rangle$ as

$$
|\psi\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle,
\qquad
|g\rangle\in G,
\quad |b\rangle\in G^\perp.
$$

The [amplitude amplification theorem](../../../../../../amplitude-amplification.md) states that for

$$
R=I_{|\psi\rangle}I_G
$$

one has, up to the irrelevant global sign $(-1)^k$,

$$
\boxed{R^k|\psi\rangle
=(-1)^k\left[
\sin((2k+1)\theta)|g\rangle
+\cos((2k+1)\theta)|b\rangle
\right]}.
$$

Thus every iteration increases the angle toward the good axis by $2\theta$ until the first overshoot.

For the proof, the plane $\operatorname{span}\{|g\rangle,|b\rangle\}$ is invariant. In its ordered basis,

$$
I_G=\begin{pmatrix}-1&0\\0&1\end{pmatrix},
\qquad
I_{|\psi\rangle}
=\begin{pmatrix}
\cos2\theta&-\sin2\theta\\
-\sin2\theta&-\cos2\theta
\end{pmatrix}.
$$

Their product is a planar rotation through $2\theta$ together with an overall sign. Applying that matrix $k$ times proves the formula, while components orthogonal to this plane never enter the initial state.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
