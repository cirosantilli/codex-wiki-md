<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Use $q\in k^\times$ and $YX=qXY$ for the [quantum plane](../../../../../quantum-plane.md). Its [monomials](../../../../../monomial.md) $X^iY^j$, $i,j\geq0$, form a [basis](../../../../../basis.md), with multiplication

$$
(X^iY^j)(X^uY^v)=q^{ju}X^{i+u}Y^{j+v}.
$$

One way to verify the [basis](../../../../../basis.md) assertion without assuming it is to define this multiplication on the [vector space](../../../../../vector-space-split.md) with the displayed formal [basis](../../../../../basis.md). This defines an [associative algebra](../../../../../associative-algebra-split.md): for a third [monomial](../../../../../monomial.md) $X^wY^z$, the two products of three [monomials](../../../../../monomial.md) have the same exponent $ju+jw+vw$ of $q$, and its generators satisfy the required relation. Conversely, the relation puts every word into this form, establishing the presentation. Order exponent pairs by the [lexicographic order](../../../../../lexicographic-order.md). The largest [monomials](../../../../../monomial.md) of two nonzero finite sums give the uniquely largest [monomial](../../../../../monomial.md) of their product, with coefficient $c d q^{ju}\ne0$. Therefore **the quantum plane is a domain**. If one allows $q=0$, the assertion fails because $YX=0$ with both factors nonzero.

A [uniform module](../../../../../uniform-module.md) is a nonzero [module](../../../../../module-mathematics.md) in which any two nonzero [submodules](../../../../../submodule.md) have nonzero intersection. Suppose the right regular [module](../../../../../module-mathematics.md) of a [right Noetherian domain](../../../../../right-noetherian-domain.md) $A$ were not a [uniform module](../../../../../uniform-module.md). Choose nonzero $a,b$ from two [right ideals](../../../../../right-ideal.md) with zero intersection. Then $aA\cap bA=0$. The [right ideals](../../../../../right-ideal.md)

$$
aA,\ baA,\ b^2aA,\ldots
$$

form a [direct sum](../../../../../direct-sum.md). For if $\sum_{i=0}^m b^ia c_i=0$, then $ac_0\in aA\cap bA$ is zero, so $c_0=0$ by the [noncommutative domain](../../../../../noncommutative-domain.md) property. Cancel the nonzero factor $b$ on the left and repeat to obtain every $c_i=0$. Each summand is nonzero, so their finite partial sums form a strictly ascending chain of [right ideals](../../../../../right-ideal.md). This contradicts the [ascending chain condition](../../../../../ascending-chain-condition.md) of a [right Noetherian ring](../../../../../right-noetherian-ring.md). Hence **$A$ is a uniform right module**.

It follows that $aA\cap sA\ne0$ whenever $a,s\ne0$: there are nonzero $u,v$ with $au=sv$. This is the [right Ore condition](../../../../../right-ore-condition.md) for the multiplicative set $S=A\setminus\{0\}$; zero numerators cause no difficulty. The [Ore localization](../../../../../ore-localization.md) theorem therefore constructs the [ring](../../../../../ring.md) of right fractions

$$
\boxed{Q=AS^{-1}=\{as^{-1}:a\in A,\ s\ne0\},\qquad A\hookrightarrow Q.}
$$

The map is injective because an element mapping to zero is annihilated on the right by some nonzero denominator, impossible in a [noncommutative domain](../../../../../noncommutative-domain.md). To make the denominator convention concrete, if $su=tv\ne0$ then

$$
as^{-1}+bt^{-1}=(au+bv)(su)^{-1}.
$$

For multiplication, choose $bu=sc$ with $u\ne0$; then

$$
(as^{-1})(bt^{-1})=ac(tu)^{-1}.
$$

Common right multiples make these operations independent of the chosen representatives. Every nonzero $as^{-1}$ has inverse $sa^{-1}$, so $Q$ is a [division ring](../../../../../division-ring.md). The original [field](../../../../../field.md) $k$ is central in $A$ and therefore in the inverses as well, making $Q$ a [division algebra](../../../../../division-algebra.md) over $k$. No commutative [fraction field](../../../../../field-of-fractions.md) construction is being assumed.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 128](../../paper-128-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
