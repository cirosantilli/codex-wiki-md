<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First use the [canonical map](../../../../../../canonical-map.md) to obtain the embedding. Its [canonical divisor](../../../../../../canonical-divisor.md) has degree six and $h^0(K_C)=4$. Over an algebraically closed ground field, every effective degree-two [divisor on an algebraic curve](../../../../../../divisor-on-an-algebraic-curve.md) $E$ satisfies $h^0(E)=1$: a second section would give a nonconstant rational function with poles bounded by $E$, hence a map $C\to\mathbb P^1$ of degree at most two. Degree one would make $C$ rational, and degree two would make it [hyperelliptic](../../../../../../hyperelliptic-curve.md), both excluded here.

The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) now gives

$$
h^0(K_C-E)=\deg(K_C-E)+1-g+h^0(E)=4+1-4+1=2.
$$

Thus the complete [linear system of divisors](../../../../../../linear-system-of-divisors.md) $|K_C|$ separates every pair of points and every tangent direction, including the tests $E=2p$. By the [length-two criterion for a very ample linear system](../../../../../../length-two-criterion-for-a-very-ample-linear-system.md), it is a [very ample linear system](../../../../../../very-ample-linear-system.md). Consequently the [canonical map](../../../../../../canonical-map.md) embeds $C$ in $\mathbb P^3$, with [degree of a projective curve](../../../../../../degree-of-a-projective-curve.md) six. Its image is a [nondegenerate projective variety](../../../../../../nondegenerate-projective-variety.md), since the four canonical sections are linearly independent.

The space of homogeneous quadrics in four variables has dimension ten, while the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) gives

$$
h^0(C,2K_C)=12+1-4=9.
$$

Restriction therefore has a nonzero kernel, giving a quadric $Q$ containing $C$. This quadric is irreducible: a reducible quadric is a union of two planes, or a double plane, and an integral curve lying in it would lie in a plane, contradicting nondegeneracy.

Similarly, homogeneous cubics form a twenty-dimensional space, whereas

$$
h^0(C,3K_C)=18+1-4=15.
$$

There are at least five independent cubics vanishing on $C$. The multiples of $Q$ by linear forms give only four dimensions, so choose a cubic $F$ vanishing on $C$ which is not divisible by $Q$.

The polynomials $Q,F$ are a [regular sequence](../../../../../../regular-sequence.md), hence their intersection $D$ is a [projective complete intersection](../../../../../../projective-complete-intersection.md) of pure dimension one and degree $2\cdot3=6$. It contains $C$, which already has degree six. The [unmixedness of a complete intersection](../../../../../../unmixedness-of-a-complete-intersection.md) excludes embedded components. Equal degrees force $C$ to be the only irreducible component and force multiplicity one at its [generic point](../../../../../../generic-point.md). By [generic reducedness with no embedded components](../../../../../../generic-reducedness-with-no-embedded-components.md), this makes $D$ reduced, so $D=C$ as schemes. **We have proved**

$$
\boxed{C\simeq V(Q,F)\subseteq\mathbb P^3,\qquad\deg Q=2,\quad\deg F=3.}
$$

This is a [canonical genus-four curve as a quadric-cubic intersection](../../../../../../canonical-genus-four-curve-as-a-quadric-cubic-intersection.md). The quadric may be smooth or a cone; the argument does not require it to be smooth. The same construction descends over the ground field when the curve is geometrically nonhyperelliptic, since the restriction maps and canonical embedding are defined there.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 20](../../../paper-20-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
