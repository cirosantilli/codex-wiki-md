<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

Sending a matrix to its last column gives the [special orthogonal sphere fibration](../../../../../special-orthogonal-sphere-fibration.md)

$$
SO(n-1)\longrightarrow SO(n)\longrightarrow S^{n-1},\qquad n\geq2.
$$

The action is transitive and the stabilizer of that column is $SO(n-1)$. Local orthonormal frames, obtained by [Gram-Schmidt process](../../../../../gram-schmidt-process.md) near a chosen unit vector, give local sections and hence local bundle trivializations. This allows the [long exact sequence of homotopy groups of a fibration](../../../../../long-exact-sequence-of-homotopy-groups-of-a-fibration.md) to be applied.

At the bottom of the induction, $SO(1)$ is a point and $SO(2)$ is the rotation circle $S^1$. For $SO(3)$, identify $\mathbb R^3$ with imaginary [quaternions](../../../../../quaternion.md). A [unit quaternion](../../../../../unit-quaternion.md) acts by $v\mapsto qvq^{-1}$, preserving length and orientation. Every rotation through angle $\theta$ about a unit imaginary axis $u$ comes from $q=\cos(\theta/2)+u\sin(\theta/2)$. The kernel is precisely $\{1,-1\}$, since a [quaternion](../../../../../quaternion.md) commuting with all imaginary [quaternions](../../../../../quaternion.md) is real. Thus this gives the twofold [covering space](../../../../../covering-space.md) $S^3\to SO(3)$. Its simply connected total space is the [universal cover](../../../../../universal-cover.md), yielding $\pi_1SO(3)=\mathbb Z/2$. Coverings induce isomorphisms on higher [homotopy groups](../../../../../homotopy-group.md), so $\pi_2SO(3)=\pi_2S^3=0$ and $\pi_3SO(3)=\pi_3S^3=\mathbb Z$.

For $n\geq4$, both $\pi_1S^{n-1}$ and $\pi_2S^{n-1}$ vanish. The [Serre fibration](../../../../../serre-fibration.md) sequence therefore identifies $\pi_1SO(n-1)$ with $\pi_1SO(n)$ and propagates vanishing of $\pi_2$. Path-connectedness also propagates from connected fiber and base. Consequently the full low-degree answer is

$$
\boxed{\pi_0SO(n)=\{*\},\quad\pi_2SO(n)=0\quad(n\geq1),\qquad
\pi_1SO(n)=\begin{cases}0,&n=1,\\\mathbb Z,&n=2,\\\mathbb Z/2,&n\geq3.\end{cases}}
$$

Here $\pi_0$ records the single connected component.

For the remaining third group use $SO(3)\to SO(4)\to S^3$. The relevant exact segment, using the supplied fourth [homotopy group](../../../../../homotopy-group.md), is

$$
\mathbb Z/2\longrightarrow\mathbb Z\longrightarrow\pi_3SO(4)\longrightarrow\mathbb Z\longrightarrow0.
$$

The first homomorphism is zero since a [torsion group](../../../../../torsion-group.md) cannot map nontrivially to $\mathbb Z$. Thus it reduces to a [short exact sequence](../../../../../short-exact-sequence.md) $0\to\mathbb Z\to\pi_3SO(4)\to\mathbb Z\to0$. These groups are abelian and the final free group has a lift of its generator, so the sequence splits. Therefore

$$
\boxed{\pi_3SO(1)=\pi_3SO(2)=0,\qquad\pi_3SO(3)=\mathbb Z,\qquad\pi_3SO(4)=\mathbb Z\oplus\mathbb Z.}
$$

These are the [low homotopy groups of special orthogonal groups](../../../../../low-homotopy-groups-of-special-orthogonal-groups.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
