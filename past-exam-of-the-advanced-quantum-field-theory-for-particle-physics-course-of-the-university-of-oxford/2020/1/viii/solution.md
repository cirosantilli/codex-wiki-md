<h1 id="1/viii/solution">Solution</h1>

↑ **Parent:** [Viii](../viii.md)

The [proper quark-gluon vertex colour factors](../../../../proper-quark-gluon-vertex-colour-factors.md) come from two [one-particle-irreducible Feynman diagrams](../../../../one-particle-irreducible-feynman-diagram.md), shown in the upper-middle and upper-right panels. One has a virtual [gluon](../../../../gluon.md) joining the open [quark](../../../../quark.md) line on opposite sides of the external [gluon](../../../../gluon.md) insertion. The other has two virtual [gluons](../../../../gluon.md) meeting the external [gluon](../../../../gluon.md) at a three-gluon [Feynman vertex](../../../../interaction-vertex.md), with their other ends joined by an internal [quark](../../../../quark.md). A [Faddeev-Popov ghost field](../../../../faddeev-popov-ghost.md) has no direct [quark](../../../../quark.md) coupling, so it supplies no additional one-loop [Feynman vertex](../../../../interaction-vertex.md) graph here.

Let $T^a$ be the Hermitian generators of the [fundamental representation](../../../../fundamental-representation.md) of $SU(N)$, with $\operatorname{tr}(T^aT^b)=\delta^{ab}/2$, $[T^a,T^b]=if^{abc}T^c$, $\sum_bT^bT^b=C_F\mathbf1$, and $f^{abc}f^{dbc}=C_A\delta^{ad}$. Here $C_F=(N^2-1)/(2N)$ and $C_A=N$ are [quadratic Casimir operators](../../../../quadratic-casimir-operator.md) evaluated in the [fundamental representation](../../../../fundamental-representation.md) and the [Adjoint representation](../../../../adjoint-representation-of-a-lie-algebra.md).

For the first graph, the ordered product is $\sum_bT^bT^aT^b$. Expand the double [commutator](../../../../commutator.md):

$$
\sum_b[T^b,[T^b,T^a]]=2C_FT^a-2\sum_bT^bT^aT^b=C_AT^a.
$$

Thus its [colour factor](../../../../color-factor.md) is

$$
\boxed{\sum_bT^bT^aT^b=\left(C_F-\frac{C_A}{2}\right)T^a=-\frac1{2N}T^a=-\frac16T^a\quad(N=3).}
$$

For the second graph choose the orientation of the three-gluon [Feynman vertex](../../../../interaction-vertex.md) so that its group tensor is $f^{abc}$ and the ordered product along the [quark](../../../../quark.md) line is $T^bT^c$. Antisymmetry removes the [anticommutator](../../../../anticommutator.md) part:

$$
\boxed{f^{abc}T^bT^c=\frac12f^{abc}[T^b,T^c]=\frac{iC_A}{2}T^a=\frac{3i}{2}T^a\quad(N=3).}
$$

The corresponding real group coefficient is $C_A/2=3/2$ after the conventional factor of $i$ is incorporated into the remaining [Feynman rules](../../../../feynman-rules.md). If the vertex is written with $if^{abc}$, its raw matrix product is instead $-C_AT^a/2$. Reversing the ordered product reverses its sign together with the orientation-dependent three-gluon [Feynman rule](../../../../feynman-rule.md); these conventions describe the same [scattering amplitude](../../../../scattering-amplitude.md). External-leg corrections and local [counterterms](../../../../counterterm.md) are separate from these two proper one-loop graphs.

## ↑ Ancestors (12)

1. [Viii](../viii.md)
2. [1](../../1.md)
3. [2020](../../../2020-split.md)
4. [Past exam of the advanced quantum field theory for particle physics course of the University of Oxford](../../../split.md)
5. [Advanced quantum field theory for particle physics course of the University of Oxford](../../../../advanced-quantum-field-theory-for-particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
