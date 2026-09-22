<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $A=k_q[x,y]$. First describe the multiplication of the [universal measuring coalgebra](../../../../../../universal-measuring-coalgebra.md) $P(A,A)$. If $C,D$ measure $A$ into itself through $p_C,p_D$, then their [tensor product](../../../../../../tensor-product.md) [coalgebra](../../../../../../coalgebra.md) measures it by

$$
(c\otimes d)(a)=p_C(c)\bigl(p_D(d)(a)\bigr).
$$

Indeed applying both measuring product rules gives the product rule for the tensor [comultiplication](../../../../../../comultiplication.md), and the unit condition follows likewise. Apply universality with $C=D=P(A,A)$: composition induces a [coalgebra](../../../../../../coalgebra.md) homomorphism $\mu:P(A,A)\otimes P(A,A)\to P(A,A)$. The identity endomorphism induces the unit $k\to P(A,A)$. Associativity and the unit laws follow by uniqueness because both candidate [coalgebra](../../../../../../coalgebra.md) homomorphisms evaluate as the same compositions of endomorphisms. Thus $P(A,A)$ is a [bialgebra](../../../../../../bialgebra.md).

The generator actions from Question 4 satisfy all defining relations of the [quantum enveloping algebra of sl2](../../../../../../quantum-enveloping-algebra-of-sl2.md), so they define an action of $U_q$ on $A$. Its skew product rules are exactly the rules from $\Delta E=E\otimes K+1\otimes E$ and $\Delta F=F\otimes1+K^{-1}\otimes F$. Products of elements satisfying the [module algebra](../../../../../../module-algebra.md) rule satisfy it as well: apply the two successive actions and use that $\Delta$ is multiplicative. Since the generators and unit satisfy it, the full action $p:U_q\to\operatorname{End}_k(A)$ is a measuring of $A$ into itself.

Universality therefore gives a unique [coalgebra](../../../../../../coalgebra.md) homomorphism $\rho:U_q\to P(A,A)$ inducing this action. To prove multiplicativity, compare the two [coalgebra](../../../../../../coalgebra.md) homomorphisms from $U_q\otimes U_q$ given by $\rho\mu_{U_q}$ and $\mu_{P}(\rho\otimes\rho)$. Both induce $(u\otimes v)(a)=u(va)$, so uniqueness makes them equal. The unit comparison is identical. Consequently

$$
\boxed{\rho:U_q\longrightarrow P(k_q[x,y],k_q[x,y])\text{ is a bialgebra homomorphism}.}
$$

This avoids assuming the universal measuring map is injective: equality is justified by its universal property for [coalgebra](../../../../../../coalgebra.md) maps.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
