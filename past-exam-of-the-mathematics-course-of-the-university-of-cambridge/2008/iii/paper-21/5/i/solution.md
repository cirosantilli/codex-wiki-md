<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $E$ be the [elliptic curve](../../../../../../elliptic-curve.md), and choose a point $O\in E(k)$ to serve as identity. Its [geometric genus](../../../../../../geometric-genus.md) is one and its [canonical divisor](../../../../../../canonical-divisor.md) $K$ has degree zero. For any divisor $D$ of degree one, the [Riemann-Roch theorem](../../../../../../riemann-roch-theorem.md) gives

$$
\ell(D)-\ell(K-D)=\deg D+1-1=1.
$$

Since $K-D$ has degree $-1$, its [Riemann-Roch space](../../../../../../riemann-roch-space.md) is zero: a nonzero section would produce an [effective divisor](../../../../../../effective-cartier-divisor.md) of negative degree. Hence $\ell(D)=1$. Choose a nonzero $f\in L(D)$. The divisor $D+(f)$ is effective of degree one, so over the algebraically closed field it is a single point $P$. Thus every degree-one [divisor class](../../../../../../divisor-class.md) has a point representative.

This representative is unique. If $P$ and $Q$ are linearly equivalent, choose $h$ with $(h)=P-Q$. Then $h\in L(Q)$. That space has dimension one and already contains the constants, so $h$ is constant and $P=Q$. Consequently

$$
\iota:E(k)\longrightarrow\operatorname{Pic}^0(E),\qquad P\longmapsto[P-O]
$$

is injective. It is also surjective: if $D$ represents a degree-zero [divisor class](../../../../../../divisor-class.md), apply the preceding result to $D+O$ to obtain its unique point representative $P$, giving $[D]=[P-O]$.

The [degree-zero Picard group of a curve](../../../../../../degree-zero-picard-group-of-a-curve.md) is a group because divisors add commutatively, [principal divisors](../../../../../../principal-divisor-on-an-algebraic-curve.md) form a subgroup, and degree passes to the quotient. Define

$$
\boxed{P\oplus Q=\iota^{-1}\bigl(\iota(P)+\iota(Q)\bigr).}
$$

Equivalently, $R=P\oplus Q$ is the unique point satisfying the [linear equivalence of divisors](../../../../../../linear-equivalence-of-divisors.md) $P+Q\sim R+O$, where the plus signs in this equivalence denote divisor addition. The zero class corresponds to $O$, so $O$ is the identity. The inverse of $P$ is the unique point $P'$ with $P+P'\sim2O$. Associativity follows because both $(P\oplus Q)\oplus R$ and $P\oplus(Q\oplus R)$ map to $\iota(P)+\iota(Q)+\iota(R)$, and $\iota$ is injective; commutativity follows in the same way. Thus this is **an abelian group structure on $E(k)$**, obtained directly by the [elliptic curve group law from Riemann-Roch](../../../../../../elliptic-curve-group-law-from-riemann-roch.md). The identity choice is part of the construction.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
