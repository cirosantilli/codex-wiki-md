<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

An [equivalence relation](../../../../../equivalence-relation.md) on $A$ is a [binary relation](../../../../../binary-relation.md) that is reflexive, symmetric and transitive: $xRx$ for every $x$; $xRy\Rightarrow yRx$; and $xRy,\ yRz\Rightarrow xRz$. Write $T=R\circ S$, using the stated order for [composition of relations](../../../../../composition-of-relations.md). Composition is associative because both possible bracketings mean that there is a two-step sequence of intermediate witnesses. [Reflexivity](../../../../../reflexive-relation.md) shows

$$
R\subseteq T,\qquad S\subseteq T,
$$

and also that $T$ is reflexive. [Transitivity](../../../../../transitive-relation.md) and [reflexivity](../../../../../reflexive-relation.md) of the original relations give $R\circ R=R$, $S\circ S=S$. Since both original relations are symmetric,

$$
T^{-1}=(R\circ S)^{-1}=S\circ R.
$$

The four parts below show that each condition is equivalent to the [commuting equivalence relations](../../../../../commuting-equivalence-relations.md) condition $R\circ S=S\circ R$.

For the integer example, put $d=\gcd(m,n)$. Membership of $(x,z)$ in the composite means that some $y$ satisfies $y-x=ma$, $z-y=nb$ for integers $a,b$. Consequently $z-x=ma+nb$ is divisible by $d$. Conversely, if $z-x$ is divisible by $d$, the [Bezout identity](../../../../../bezout-identity.md) expresses it as $ma+nb$; setting $y=x+ma$ provides the required witness. Thus

$$
\boxed{R\circ S=\{(x,z)\in\mathbb Z^2:x\equiv z\pmod d\}.}
$$

Reversing the roles of $m,n$ gives exactly the same [modular congruence](../../../../../modular-congruence.md) relation, hence $R\circ S=S\circ R$. This verifies all four conditions and identifies their common smallest [equivalence relation](../../../../../equivalence-relation.md) explicitly.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
