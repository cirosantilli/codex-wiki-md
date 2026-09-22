<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the printed congruence entrywise in the integer lattice:

$$
a,d\in1+2\mathbb Z,\qquad b,c\in2\mathbb Z.
$$

It then defines the usual level-two [principal congruence subgroup](../../../../../../principal-congruence-subgroup.md) of $\mathrm{SL}_2(\mathbb Z)$, despite the PDF's ambient $\mathrm{SL}_2(\mathbb R)$. A literal ideal congruence inside $\mathbb R$ would be vacuous because $2\mathbb R=\mathbb R$, and would make the asserted conclusion false. The integer-lattice interpretation is essential.

Pass to $\overline{\Gamma(2)}=\Gamma(2)/\{\pm I\}$, which has exactly the same action. Reduction modulo two maps the [modular group](../../../../../../modular-group.md) onto $\mathrm{SL}_2(\mathbb F_2)$, a group of order six: the reductions of $S$ and $T$ generate it. Its kernel is $\overline{\Gamma(2)}$, so the [index of a subgroup](../../../../../../index-of-a-subgroup.md) is six. The [standard fundamental domain of the modular group](../../../../../../standard-fundamental-domain-of-the-modular-group.md) has [hyperbolic area](../../../../../../hyperbolic-area.md) $\pi/3$, and hence the quotient has [hyperbolic area](../../../../../../hyperbolic-area.md) $2\pi$.

There are no nonidentity [elliptic Möbius transformations](../../../../../../elliptic-element-of-psl2-r.md) in $\overline{\Gamma(2)}$. An integral matrix representing an [elliptic Möbius transformation](../../../../../../elliptic-element-of-psl2-r.md) has [trace](../../../../../../matrix-trace.md) $0$ or $\pm1$. Here the [trace](../../../../../../matrix-trace.md) is even, excluding $\pm1$; [trace](../../../../../../matrix-trace.md) zero would give $d=-a$ and $1=-a^2-bc\equiv-1\pmod4$, impossible. Thus the effective action is a free [properly discontinuous group action](../../../../../../properly-discontinuous-group-action.md), and the quotient is a [Riemann surface](../../../../../../riemann-surfaces.md).

A [cusp of a modular group](../../../../../../cusp-of-a-modular-group.md) is represented by a rational boundary point. Their orbits correspond to

$$
\mathrm{SL}_2(\mathbb F_2)/\langle\overline T\rangle,
$$

which has $6/2=3$ elements. They are represented by $\infty,0,1$, or by the three nonzero parity vectors of a primitive numerator-denominator pair. Each [width of a cusp](../../../../../../width-of-a-cusp.md) is two. A union of six copies of the [standard fundamental domain of the modular group](../../../../../../standard-fundamental-domain-of-the-modular-group.md) gives a fundamental region for this subgroup. Removing small [horocycle](../../../../../../horocycle.md) neighbourhoods of its cusps leaves a [compact](../../../../../../compact-space.md) core. Adding one point at each [cusp of a modular group](../../../../../../cusp-of-a-modular-group.md), using the local parameter $e^{\pi i z}$ after moving that cusp to infinity, gives a [compact](../../../../../../compact-space.md) [Riemann surface](../../../../../../riemann-surfaces.md) $\overline X$.

For a finite-area [hyperbolic surface](../../../../../../hyperbolic-surface.md) of [genus](../../../../../../genus-of-a-surface.md) $g$ with $r$ cusps, the [Gauss-Bonnet theorem](../../../../../../gauss-bonnet-theorem.md) gives area $2\pi(2g-2+r)$. Thus $2\pi=2\pi(2g-2+3)$ and $g=0$. A [compact](../../../../../../compact-space.md) [genus](../../../../../../genus-of-a-surface.md)-zero [Riemann surface](../../../../../../riemann-surfaces.md) is the [Riemann sphere](../../../../../../riemann-sphere.md), by the [uniformization theorem](../../../../../../uniformization-theorem.md). A [Möbius transformation](../../../../../../mobius-transformation.md) sends the three added points to $0,1,\infty$. Restricting it gives

$$
\boxed{\mathbb H/\Gamma(2)\cong\mathbb P^1\setminus\{0,1,\infty\}
=\mathbb C\setminus\{0,1\}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 132](../../../paper-132-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
