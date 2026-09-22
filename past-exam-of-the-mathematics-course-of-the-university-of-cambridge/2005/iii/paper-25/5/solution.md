<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The smooth [h-cobordism theorem](../../../../../h-cobordism-theorem.md) states: if $(W;M_0,M_1)$ is a compact smooth [h-cobordism](../../../../../h-cobordism.md), $\dim W\ge6$, and its connected boundary [manifolds](../../../../../topological-manifold.md) are simply connected, then there is a [diffeomorphism](../../../../../diffeomorphism.md) $W\cong M_0\times[0,1]$ restricting to the prescribed identification on $M_0$. In particular $M_0$ and $M_1$ are [diffeomorphic](../../../../../diffeomorphism.md). Being an [h-cobordism](../../../../../h-cobordism.md) means that both inclusions $M_i\hookrightarrow W$ are [homotopy equivalences](../../../../../homotopy-equivalence.md); their fundamental groups then also identify with that of $W$.

The homotopy-equivalence condition is necessary for a [trivial cobordism](../../../../../trivial-cobordism.md): each end of a cylinder is a deformation retract, by $(x,t)\mapsto(x,(1-s)t)$ for the incoming end and $(x,t)\mapsto(x,(1-s)t+s)$ for the outgoing end. Its [relative homology](../../../../../relative-homology.md) with respect to either end is consequently zero. Compactness is also necessary for a product with a closed compact end. The dimensional bound and simple connectivity are not necessary for an individual [cobordism](../../../../../cobordism.md) to be a product. The cylinder $S^2\times[0,1]$ is a simply connected [trivial cobordism](../../../../../trivial-cobordism.md) of dimension three; and, in the theorem's dimension range, $(S^1\times S^4)\times[0,1]$ is a six-dimensional [trivial cobordism](../../../../../trivial-cobordism.md) with [fundamental group](../../../../../fundamental-group.md) $\mathbb Z$. These prove the two non-necessity assertions explicitly, while the inclusion argument proves necessity of the h-condition.

For the remaining claims, use a [cobordism Morse function](../../../../../cobordism-morse-function.md): its two regular boundary levels are zero and one, and all [critical points](../../../../../critical-point.md) are interior. An arbitrary function with unrelated boundary values would not have the relative handle-count property. The relative [Morse chain complex](../../../../../morse-chain-complex.md) for $(W,M_0)$ has one generator per [critical point](../../../../../critical-point.md), in its [Morse index](../../../../../morse-index.md). Thus

$$
\chi(W,M_0)=\sum_{r\in\operatorname{Crit}(f)}(-1)^{\operatorname{ind}(r)}.
$$

A [trivial cobordism](../../../../../trivial-cobordism.md) has zero [relative homology](../../../../../relative-homology.md), hence zero relative [Euler characteristic](../../../../../euler-characteristic.md). Modulo two the displayed sum is the number of [critical points](../../../../../critical-point.md). An odd number makes it odd, and therefore nonzero. This proves **an odd-critical-point [cobordism](../../../../../cobordism.md) is not trivial**.

With precisely two [critical points](../../../../../critical-point.md) of indices $\lambda\le\mu$, a [trivial cobordism](../../../../../trivial-cobordism.md) requires the two-generator relative complex to be acyclic over $\mathbb Z$. Equal indices leave a rank-two [homology](../../../../../homology-split.md) group; a gap of more than one leaves both generators with zero possible differential. Therefore **$\mu=\lambda+1$ is necessary**. The remaining two-term complex is

$$
0\longrightarrow\mathbb Z q\xrightarrow{\times a}\mathbb Z p\longrightarrow0.
$$

Choose a transverse [gradient-like vector field](../../../../../gradient-like-vector-field.md). A nonzero differential requires the index-$\mu$ point to be above the index-$\lambda$ point; otherwise no descending connecting trajectories exist. In a common regular level between them, the [belt sphere](../../../../../belt-sphere.md) $S_U(p)$ has dimension $d-\lambda-1$, and the [attaching sphere](../../../../../attaching-sphere.md) $S_L(q)$ has dimension $\mu-1=\lambda$, where $d=\dim W$. Their dimensions add to $d-1$, the level's dimension, so their transverse intersection consists of points. Each intersection is one descending trajectory from $q$ to $p$, modulo time translation. Orient the [attaching sphere](../../../../../attaching-sphere.md) and use an [orientation of a vector space](../../../../../orientation-of-a-vector-space.md) on the [handle](../../../../../handle.md) core to coorient the [belt sphere](../../../../../belt-sphere.md); the resulting signed count is the cellular boundary coefficient

$$
a=S_U(p)\cdot S_L(q).
$$

The two [homology](../../../../../homology-split.md) groups are the kernel and cokernel of multiplication by $a$. They vanish precisely when $a$ is a unit of $\mathbb Z$. Consequently

$$
\boxed{\mu=\lambda+1,\qquad S_U(p)\cdot S_L(q)=\pm1}
$$

are necessary. This proves the [two-critical-point obstruction to a trivial cobordism](../../../../../two-critical-point-obstruction-to-a-trivial-cobordism.md); it makes an algebraic incidence statement and does not assume that an algebraic count of one automatically supplies geometric [handle](../../../../../handle.md) cancellation.

For an explicit nontrivial [cobordism](../../../../../cobordism.md) from $S^3$ to itself, attach two zero-framed [two-handles](../../../../../two-handle.md) to the outgoing end of $S^3\times[0,1]$ along the standard [Hopf link](../../../../../hopf-link.md). Its two components are unknots with linking number one. This realizes two successive $(2,2)$ surgeries, as suggested by the hint. The outgoing boundary is again $S^3$, and this can be checked geometrically: the Hopf-link exterior is $T^2\times[0,1]$, and each component's zero-framing longitude is the other's meridian. Filling along these two slopes glues two solid [tori](../../../../../torus.md) with meridians intersecting once, the standard genus-one Heegaard decomposition of $S^3$. Thus [zero surgery on the Hopf link](../../../../../zero-surgery-on-the-hopf-link.md) does return the three-sphere, not just an unspecified [homology](../../../../../homology-split.md) [sphere](../../../../../sphere.md).

The trace has only the two added index-two [handles](../../../../../handle.md). Its relative cellular complex has $C_2(W,S^3)=\mathbb Z^2$ and all other groups zero, so

$$
\boxed{H_2(W,S^3;\mathbb Z)=\mathbb Z^2\ne0.}
$$

It cannot be a product cylinder. Equivalently this trace is $S^2\times S^2$ with two disjoint open four-balls removed: the usual [handle](../../../../../handle.md) presentation of $S^2\times S^2$ has one [zero-handle](../../../../../zero-handle.md), the two zero-framed Hopf-linked [two-handles](../../../../../two-handle.md), and one four-handle. Removing the bottom and top balls exposes the two three-sphere ends. The relative-homology calculation alone already proves **the requested [cobordism](../../../../../cobordism.md) is nontrivial**.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
