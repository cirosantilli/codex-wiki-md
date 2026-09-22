<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Assume first $0<k<N$. Define the orthonormal [quantum states](../../../../../../quantum-state.md)

$$
|B\rangle=\frac1{\sqrt{N-k}}\sum_{x\notin G}|x\rangle,\qquad |G\rangle=\frac1{\sqrt k}\sum_{x\in G}|x\rangle,
$$

and $\theta\in(0,\pi/2)$ by $\sin\theta=\sqrt{k/N}$. The relevant [invariant subspace](../../../../../../invariant-subspace.md) is the two-dimensional [span](../../../../../../linear-span.md) of these [quantum states](../../../../../../quantum-state.md), not the entire [Hilbert space](../../../../../../hilbert-space-split.md). The [uniform quantum superposition](../../../../../../uniform-quantum-superposition.md) is $|\psi_0\rangle=\cos\theta|B\rangle+\sin\theta|G\rangle$.

In the ordered [orthonormal basis](../../../../../../orthonormal-basis.md) $(|B\rangle,|G\rangle)$, the [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md) is the [reflection operator](../../../../../../reflection-operator.md) $I_G=\operatorname{diag}(1,-1)$. Since $I_0=I-2|0^n\rangle\langle0^n|$, conjugation by the [Walsh-Hadamard transform](../../../../../../walsh-hadamard-transform.md) gives the [Grover diffusion operator](../../../../../../grover-diffusion-operator.md)

$$
D=-H_nI_0H_n=2|\psi_0\rangle\langle\psi_0|-I.
$$

It is the reflection in the line through $|\psi_0\rangle$. The product of these two [reflection operators](../../../../../../reflection-operator.md) is a [rotation matrix](../../../../../../rotation-matrix.md) by $2\theta$ toward the marked [quantum state](../../../../../../quantum-state.md):

$$
Q=DI_G=\begin{pmatrix}\cos2\theta&-\sin2\theta\\\sin2\theta&\cos2\theta\end{pmatrix},\qquad Q^j|\psi_0\rangle=\cos((2j+1)\theta)|B\rangle+\sin((2j+1)\theta)|G\rangle.
$$

Thus the [Born rule](../../../../../../born-rule.md) gives $P_j=\sin^2((2j+1)\theta)$. Choose a nonnegative integer $j_*$ nearest to $\pi/(4\theta)-1/2$. Rounding changes the angle from $\pi/2$ by at most $\theta$, so

$$
\boxed{P_{j_*}\geq\cos^2\theta=1-\frac kN,\qquad j_*=O\!\left(\sqrt{\frac Nk}\right).}
$$

Each [Grover search algorithm](../../../../../../grover-s-algorithm.md) iteration uses one [marked-state phase oracle](../../../../../../marked-state-phase-oracle.md) query; all other gates are known. A final [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) therefore produces a uniformly chosen marked item, conditional on success, with probability better than one half when $k<N/2$. This uses the supplied marked count $k$ to select the stopping time; an unknown $k$ needs an additional search schedule or counting procedure. If $k=N$, no oracle query is needed; if $k=0$, no marked item exists, so a successful search is impossible.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
