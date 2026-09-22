<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\Pi_{\mathcal G}$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the good [linear subspace](../../../../../../vector-subspace.md) and write

$$
|\psi\rangle
=\sin\theta\,|\psi_G\rangle
+\cos\theta\,|\psi_B\rangle,
\qquad
\sin^2\theta=\langle\psi|\Pi_{\mathcal G}|\psi\rangle,
$$

where the two displayed states are normalized projections into $\mathcal G$ and $\mathcal G^\perp$. Define the [reflections](../../../../../../reflection-in-a-hyperplane.md)

$$
R_G=I-2\Pi_{\mathcal G},
\qquad
R_\psi=2|\psi\rangle\langle\psi|-I.
$$

The [amplitude amplification](../../../../../../amplitude-amplification.md) iterate $Q=R_\psi R_G$ preserves the good-bad plane, and its $k$th iterate satisfies

$$
Q^k|\psi\rangle
=\sin((2k+1)\theta)|\psi_G\rangle
+\cos((2k+1)\theta)|\psi_B\rangle.
$$

**Thus repeated reflections rotate amplitude toward the good subspace, reaching constant success probability after $O(1/\sin\theta)$ iterations.**

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
