<h1 id="4/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\Pi_g$ project onto the good-output subspace and let $|g\rangle=|\Psi_g\rangle$, $|b\rangle=|\Psi_b\rangle$. They are orthonormal because their supporting [computational basis](../../../../../../computational-basis.md) strings are disjoint. The verification [unitary operator](../../../../../../unitary-operator.md) is $V=I-2\Pi_g$, so $V|g\rangle=-|g\rangle$ and $V|b\rangle=|b\rangle$.

Also $V_0=I-2|0\rangle\langle0|$. Since $A|0\rangle=|\Psi\rangle$, conjugating gives $AV_0A^\dagger=I-2|\Psi\rangle\langle\Psi|$. Thus

$$
Q=(2|\Psi\rangle\langle\Psi|-I)V.
$$

Both reflections preserve the span of $|g\rangle$ and $|b\rangle$: $V$ is diagonal there, and the other reflection only adds a multiple of $|\Psi\rangle$, already in that span. Direct substitution of $|\Psi\rangle=\sqrt p\,|g\rangle+\sqrt{1-p}\,|b\rangle$ yields

$$
\boxed{Q|g\rangle=(1-2p)|g\rangle-2\sqrt{p(1-p)}|b\rangle,\qquad Q|b\rangle=2\sqrt{p(1-p)}|g\rangle+(1-2p)|b\rangle.}
$$

The minus sign in the first image follows from applying $V$ before the state reflection. In the ordered basis $(|b\rangle,|g\rangle)$ the [matrix](../../../../../../matrix.md) is

$$
Q=\begin{pmatrix}1-2p&-2\sqrt{p(1-p)}\\2\sqrt{p(1-p)}&1-2p\end{pmatrix}.
$$

This exhibits the invariant plane without assumptions about the action of $A$ on the other input basis vectors.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [4](../../4.md)
3. [Paper 53](../../../paper-53-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
