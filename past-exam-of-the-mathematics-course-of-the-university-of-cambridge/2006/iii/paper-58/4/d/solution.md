<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Now $|a\rangle=|\psi\rangle$. Suppose $0<m<N$, and normalize the [orthogonal](../../../../../../orthogonal-vectors.md) good and bad components:

$$
|g\rangle=|\psi_1\rangle/\sin\chi,\qquad
|b\rangle=|\psi_0\rangle/\cos\chi,\qquad
|\psi\rangle=\sin\chi|g\rangle+\cos\chi|b\rangle.
$$

Their disjoint computational supports make $(|g\rangle,|b\rangle)$ an orthonormal basis. For $s=\sin\chi,c=\cos\chi$, the [two-dimensional matrix for phase amplitude amplification](../../../../../../two-dimensional-matrix-for-phase-amplitude-amplification.md) is

$$
\boxed{Q=-\begin{pmatrix}
t(c^2+ps^2)&(p-1)sc\\
t(p-1)sc&s^2+pc^2
\end{pmatrix}_{(g,b)}.}
$$

To obtain its first column, the marked phase first multiplies $|g\rangle$ by $t$, then $I+(p-1)|\psi\rangle\langle\psi|$ adds its projection onto $|\psi\rangle$; the second column is obtained similarly without $t$. This also proves unitarity: the rank-one phase has [eigenvalues](../../../../../../eigenvalue.md) $p,1$ on this plane, and the marked phase has [eigenvalues](../../../../../../eigenvalue.md) $t,1$, all of unit modulus. Their negative product is unitary for any real phases.

Using the unnormalized pair $(|\psi_1\rangle,|\psi_0\rangle)$ instead would produce a differently scaled matrix, which is not in general unitary in the ordinary Euclidean metric. At $m=0$ or $m=N$ one component vanishes and the relevant search space is one-dimensional.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 58](../../../paper-58-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
