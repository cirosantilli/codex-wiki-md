<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Assume $R$ is a nonzero unital [ring](../../../../../ring.md) and all its [modules](../../../../../module-mathematics.md) are unital. Order the proper [left ideals](../../../../../left-ideal.md) by inclusion. A chain has an upper bound given by its union, which is still a proper [left ideal](../../../../../left-ideal.md): if it contained $1$, one member of the chain would contain $1$ and be all of $R$. The family is nonempty because it contains $0$. The [Zorn lemma](../../../../../zorn-s-lemma.md) gives a maximal proper [left ideal](../../../../../left-ideal.md) $L$. The nonzero quotient $R/L$ has no proper nonzero [submodules](../../../../../submodule.md), because its [submodules](../../../../../submodule.md) correspond to [left ideals](../../../../../left-ideal.md) between $L$ and $R$. Thus **$R/L$ is a simple left module**. The nonzero-ring qualification is necessary: the zero [ring](../../../../../ring.md) has no nonzero unital [simple module](../../../../../irreducible-module.md).

Define the [Jacobson radical](../../../../../jacobson-radical.md) $J(R)$ as the intersection of all maximal [left ideals](../../../../../left-ideal.md). It is equivalently the intersection of the ideals $\operatorname{Ann}_R(S)$ over all [simple modules](../../../../../irreducible-module.md), where $\operatorname{Ann}$ is the [annihilator of a module](../../../../../annihilator-of-a-module.md). To verify this equivalence, for a nonzero vector $v$ in a [simple module](../../../../../irreducible-module.md) $S$, the surjection $R\to S$, $r\mapsto rv$, has a maximal left-ideal kernel. Thus $x\in J(R)$ implies $xv=0$ for every $v$ in every [simple module](../../../../../irreducible-module.md). Conversely, if $x$ annihilates all [simple modules](../../../../../irreducible-module.md), it annihilates $1+L$ in every $R/L$, so $x\in L$. An [annihilator of a module](../../../../../annihilator-of-a-module.md) is a two-sided [ideal](../../../../../ideal.md); this description therefore proves that $J(R)$ is a two-sided [ideal](../../../../../ideal.md).

For the forward implication of the [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md), first let $y\in J(R)$. If $R(1-y)$ were a proper [left ideal](../../../../../left-ideal.md), it would lie in a maximal one $L$. Both $y$ and $1-y$ would belong to $L$, an impossibility. Hence $c(1-y)=1$ for some $c\in R$. A left inverse alone does not yet establish that $1-y$ is a [unit](../../../../../unit-in-a-ring.md) in a general noncommutative [ring](../../../../../ring.md). However, $c=1+cy$, with $cy\in J(R)$, so the same argument gives $d c=1$ for some $d$. Multiplying $c(1-y)=1$ by $d$ on the left gives $d=1-y$. Therefore $(1-y)c=dc=1$ as well. This proves that $1-y$ is a [unit](../../../../../unit-in-a-ring.md).

For $x\in J(R)$, its two-sided-ideal property gives $axb\in J(R)$ for all $a,b$, so $1-axb$ is a [unit](../../../../../unit-in-a-ring.md). Conversely, if $x\notin J(R)$, choose a maximal [left ideal](../../../../../left-ideal.md) $L$ with $x\notin L$. Then $L+Rx=R$, so $l+ax=1$ for some $l\in L$, $a\in R$. Hence $1-ax=l\in L$ is not a [unit](../../../../../unit-in-a-ring.md): if it were invertible, multiplying it on the left by its inverse would put $1$ in $L$. Taking $b=1$ contradicts the given unit property. We have proved

$$
\boxed{J(R)=\{x\in R:1-axb\text{ is a unit for every }a,b\in R\}.}
$$

Finally let $R$ be [commutative](../../../../../commutativity.md) and $I$ an [ideal](../../../../../ideal.md). The set $S=1+I$ contains $1$, and

$$
(1+i)(1+j)=1+(i+j+ij)\in1+I,
$$

so it is a [multiplicative subset](../../../../../multiplicatively-closed-set.md). In the [localization of a module](../../../../../localization-of-a-module.md) $I_S\subseteq R_S$, any element is $i/s$ with $i\in I$ and $s\in S$. For any $r/t\in R_S$,

$$
1-\frac rt\frac is=\frac{ts-ri}{ts}.
$$

Both $ts$ and $ts-ri$ lie in $S$, since $ts\in1+I$ and $ri\in I$. The fraction is consequently a [unit](../../../../../unit-in-a-ring.md) in $R_S$. In a [commutative ring](../../../../../commutative-ring.md), the product of any two coefficients is again a single coefficient, so the proved [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md) applies to all expressions $1-a(i/s)b$. Thus

$$
\boxed{I_S\subseteq J(R_S).}
$$

This proves [localization away from one plus an ideal lies in the Jacobson radical](../../../../../localization-away-from-one-plus-an-ideal-lies-in-the-jacobson-radical.md). If $I=R$, then $0\in S$, $R_S=0$, and the inclusion holds trivially.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
