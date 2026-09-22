<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Put $O=0_E$. Choose rational projective coordinates in which $O=(0:1:0)$ and its tangent is $Z=0$. Because $O$ is an [inflection point of a plane cubic](../../../../../../inflection-point-of-a-plane-cubic.md), that tangent intersects the cubic in the divisor $3O$. Consequently its cubic equation has the form

$$
aX^3+bY^2Z+cXYZ+dX^2Z+eYZ^2+fXZ^2+gZ^3=0.
$$

Here $a\ne0$, since the restriction to $Z=0$ is a nonzero multiple of $X^3$, and $b\ne0$, since smoothness at $O$ requires a nonzero $Z$-derivative there. Completing the square in $Y$, by the rational linear change $Y'=Y+(cX+eZ)/(2b)$, gives on $Z=1$

$$
y'^2=c_0x^3+c_1x^2+c_2x+c_3,\qquad c_0\in\mathbb Q^*.
$$

Set $x'=c_0x$ and $y''=c_0y'$. Then

$$
\boxed{y''^2=x'^3+c_1x'^2+c_0c_2x'+c_0^2c_3.}
$$

These are invertible rational projective coordinate changes, and $O$ remains the unique point at infinity. Smoothness ensures that the resulting monic cubic has no repeated root. Thus this is a [Weierstrass equation of an elliptic curve](../../../../../../weierstrass-equation-of-an-elliptic-curve.md), without requiring any extraction of a square or cube root in $\mathbb Q$.

On this model write $-(x,y)=(x,-y)$ and $-O=O$. To add $P,Q$, take their joining line, or the tangent if $P=Q$, and let $R$ be the third intersection counted with multiplicity. Define

$$
\boxed{P+Q=-R.}
$$

For a vertical line its third intersection is $O$, so $P+(-P)=O$. The line through $O$ and an affine point is vertical, giving $P+O=P$. The tangent at $O$ has triple contact, giving $O+O=O$. This is the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md).

If $P,Q$ are rational, their joining line or tangent is rational. Its residual intersection point is rational: substituting the line in the cubic leaves a cubic whose other two roots, counted with multiplicity, are rational. Thus addition preserves $E(\mathbb Q)$. The construction is symmetric in $P,Q$, so it is commutative.

For associativity, use [divisor classes](../../../../../../divisor-class.md). A smooth plane cubic has [geometric genus](../../../../../../geometric-genus.md) $1$, by the [genus-degree formula](../../../../../../genus-degree-formula.md). The [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) says that a divisor of degree $1$ on a genus-one curve has a one-dimensional space of sections. Therefore every degree-zero [divisor class](../../../../../../divisor-class.md) is uniquely represented by $P-O$: add $O$, take its unique effective degree-one representative, and then subtract $O$. Uniqueness also follows because a nonconstant function with its only pole a simple pole at $Q$ would contradict $\ell(Q)=1$.

Every line section is linearly equivalent to the tangent section $3O$. Thus, whenever $P,Q,R$ are collinear, including tangencies,

$$
[P-O]+[Q-O]+[R-O]=0\quad\text{in }\operatorname{Pic}^0(E).
$$

A vertical section gives $[(-R)-O]=-[R-O]$. Hence the [chord-and-tangent group law](../../../../../../chord-and-tangent-group-law.md) becomes ordinary addition in the degree-zero [Picard group](../../../../../../picard-group.md) under the injective correspondence $P\mapsto[P-O]$. Associativity follows from associativity in that abelian group. Together with closure, identity and inverses already checked, this proves that **$E(\mathbb Q)$ is an abelian group**.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 125](../../../paper-125-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
