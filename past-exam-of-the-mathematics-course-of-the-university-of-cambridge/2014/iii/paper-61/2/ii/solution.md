<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\Pi_G$ be the [orthogonal projection](../../../../../../orthogonal-projection.md) onto the good [vector subspace](../../../../../../vector-subspace.md) $G$, and let the normalized input be $|\psi\rangle$. Set $p=\|\Pi_G\psi\|^2=\sin^2\theta$ with $0<\theta<\pi/2$, and define

$$
|g\rangle=\frac{\Pi_G|\psi\rangle}{\sqrt p},\qquad
|b\rangle=\frac{(I-\Pi_G)|\psi\rangle}{\sqrt{1-p}},\qquad
|\psi\rangle=\sin\theta|g\rangle+\cos\theta|b\rangle.
$$

Assuming coherent access to the two reflections, the [amplitude amplification theorem](../../../../../../amplitude-amplification.md) states that

$$
Q=(2|\psi\rangle\langle\psi|-I)(I-2\Pi_G)
$$

preserves the plane spanned by $|g\rangle,|b\rangle$ and acts as a rotation, giving

$$
\boxed{Q^j|\psi\rangle=\sin((2j+1)\theta)|g\rangle+
\cos((2j+1)\theta)|b\rangle}.
$$

Hence the good-outcome probability is $\sin^2((2j+1)\theta)$. When $p$ is known, choose the nearest nonnegative integer to $\pi/(4\theta)-1/2$. The resulting angle is within $\theta$ of $\pi/2$, so the good probability is at least $\cos^2\theta=1-p$. For small $p$ this is close to one and requires $O(1/\sqrt p)$ iterations. Exact success occurs when $(2j+1)\theta=\pi/2$. Known $p$ also allows [exact amplitude amplification](../../../../../../exact-amplitude-amplification.md) by [ancilla qubit](../../../../../../ancilla-qubit.md) dilution or selective phase adjustment when ordinary integer iterations would overshoot.

If $|\psi\rangle=A|0\rangle$ has a known coherent preparation, its reflection is implemented with $A$, $A^\dagger$ and a zero-state phase flip. A coherent membership test supplies the reflection about $G$. Merely possessing an unknown copy of $|\psi\rangle$ does not automatically supply its reflection. For $p=1$ the state is already good; for $p=0$ this two-reflection construction cannot generate a good component. These cases delimit the theorem's algorithmic assumptions.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
