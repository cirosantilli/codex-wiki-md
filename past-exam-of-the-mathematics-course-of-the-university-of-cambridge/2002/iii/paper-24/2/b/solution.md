<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use [two-isogeny descent](../../../../../../two-isogeny-descent.md) with $a=-7$, $b=12$, so the partner [elliptic curve](../../../../../../elliptic-curve.md) is $E':Y^2=X^3+14X^2+X$. On $E$, a negative $x$ would make $x(x-3)(x-4)$ negative. Hence the [prime-support bound in two-isogeny descent](../../../../../../prime-support-bound-in-two-isogeny-descent.md) restricts the [square class](../../../../../../square-class.md) image to $\{1,2,3,6\}$. All four occur: the identity gives $1$, and the [rational points](../../../../../../rational-point.md) $(2,2)$, $(0,0)$, $(6,6)$ give respectively $2$, $12\equiv3$, and $6$ in $\mathbb Q^*/\mathbb Q^{*2}$. Thus $|\alpha E(\mathbb Q)|=4$.

For the partner, $b'=1$, so its [square class](../../../../../../square-class.md) image is contained in $\{1,-1\}$. A realization of $-1$ would yield coprime integers $U,V$, not both zero, satisfying

$$
N^2=-U^4+14U^2V^2-V^4.
$$

If exactly one of $U,V$ is odd, the right side is $3$ modulo four, which is not a square. If both are odd, $U^4\equiv V^4\equiv1\pmod {16}$ and $14U^2V^2\equiv14\pmod {16}$, so the right side is $12$ modulo sixteen, again impossible. Both even is excluded by coprimality. This proves the [negative unit obstruction for the fourteen-coefficient isogeny cover](../../../../../../negative-unit-obstruction-for-the-fourteen-coefficient-isogeny-cover.md); the identity realizes $1$, so $|\alpha'E'(\mathbb Q)|=1$.

The [two-isogeny rank formula](../../../../../../square-class-index-formula-for-two-isogeny-descent.md) now gives $2^r=4\cdot1/4=1$. Consequently this is the [rank-zero elliptic curve with roots zero three and four](../../../../../../rank-zero-elliptic-curve-with-roots-zero-three-and-four.md):

$$
\boxed{\operatorname{rank}E(\mathbb Q)=0.}
$$

The displayed nonzero-ordinate points are therefore [torsion points of an elliptic curve](../../../../../../torsion-point-of-an-elliptic-curve.md), rather than evidence of positive rank. In fact doubling either $(2,2)$ or $(6,6)$ gives $(4,0)$, so both have order four.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
