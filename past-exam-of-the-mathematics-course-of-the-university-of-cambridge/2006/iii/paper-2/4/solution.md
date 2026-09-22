<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

A [filtration of a ring](../../../../../filtration-of-a-ring.md) is an exhaustive increasing family of additive subgroups $F_iR$, indexed by the integers, with $1\in F_0R$ and $F_iR\,F_jR\subseteq F_{i+j}R$. A compatible [filtration of a module](../../../../../filtration-of-a-module.md) on a right [module](../../../../../module-mathematics.md) satisfies $F_iM\,F_jR\subseteq F_{i+j}M$. The [associated graded module](../../../../../associated-graded-module.md) has components $F_iM/F_{i-1}M$, and its action by the [associated graded ring](../../../../../associated-graded-ring.md) is

$$
(m+F_{i-1}M)(r+F_{j-1}R)=mr+F_{i+j-1}M.
$$

Changing either representative changes the product only by an element of $F_{i+j-1}M$, so the action is well-defined.

The [subspace filtration](../../../../../subspace-filtration.md) on $N$ is $F_iN=N\cap F_iM$. The [quotient filtration](../../../../../quotient-filtration.md) is $F_i(M/N)=(F_iM+N)/N$. Inclusion induces an [injective](../../../../../injective-function.md) map $\operatorname{gr}N\to\operatorname{gr}M$, and the quotient induces a [surjective](../../../../../surjective-function.md) map to $\operatorname{gr}(M/N)$. If $m\in F_iM$ maps to zero in its degree-$i$ quotient, write $m=n+m'$ with $n\in N$ and $m'\in F_{i-1}M$. Then $n\in N\cap F_iM$, so the kernel is exactly the image of $\operatorname{gr}N$. We have the [short exact sequence](../../../../../short-exact-sequence.md)

$$
\boxed{0\longrightarrow\operatorname{gr}N
\longrightarrow\operatorname{gr}M
\longrightarrow\operatorname{gr}(M/N)\longrightarrow0},
$$

which is [exactness of associated graded modules for induced filtrations](../../../../../exactness-of-associated-graded-modules-for-induced-filtrations.md).

For the negative case, $F_iR=R$ for $i\geq0$. Completeness means that $R\to\varprojlim_q R/F_{-q}R$ is an [isomorphism](../../../../../isomorphism.md); in particular the [filtration of a ring](../../../../../filtration-of-a-ring.md) is separated. If $x\in F_{-1}R$ and $r\in R$, then $(xr)^q\in F_{-q}R$. The [geometric series](../../../../../geometric-series.md)

$$
\sum_{q=0}^{\infty}(xr)^q
$$

converges in the [complete negative filtration](../../../../../complete-negative-filtration.md) and is a two-sided inverse of $1-xr$, by the finite geometric identity and continuity of multiplication. The [unit criterion for the Jacobson radical](../../../../../unit-criterion-for-the-jacobson-radical.md) now gives

$$
\boxed{F_{-1}R\subseteq J(R)}.
$$

Let $I$ be any [right ideal](../../../../../right-ideal.md). The [associated graded module](../../../../../associated-graded-module.md) $\operatorname{gr}I$ for its [subspace filtration](../../../../../subspace-filtration.md) is a [homogeneous ideal](../../../../../homogeneous-ideal.md) on the right in $\operatorname{gr}R$. If $\operatorname{gr}R$ is a [right Noetherian ring](../../../../../right-noetherian-ring.md), choose homogeneous generators that lift to $x_1,\ldots,x_s\in I$, with degrees $d_1,\ldots,d_s\leq0$.

For $x\in I\cap F_dR$, cancel its degree-$d$ symbol by a sum $\sum_i x_i a_{i,0}$ with $a_{i,0}\in F_{d-d_i}R$. The remainder belongs to $I\cap F_{d-1}R$. Repeat the cancellation in each succeeding degree. After $q$ steps,

$$
x-\sum_i x_i\sum_{j=0}^{q-1}a_{i,j}\in F_{d-q}R,
\qquad a_{i,j}\in F_{d-j-d_i}R.
$$

For every $i$, the coefficient series converges to some $a_i\in R$ by completeness. Passing to the limit gives $x=\sum_i x_i a_i$. Thus these finitely many $x_i$ generate the actual [right ideal](../../../../../right-ideal.md) $I$; no assumption that $I$ is closed is needed. Since every [right ideal](../../../../../right-ideal.md) is finitely generated, **$R$ is right Noetherian**, by [complete negative filtered-graded transfer of Noetherianity](../../../../../complete-negative-filtered-graded-transfer-of-noetherianity.md).

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 2](../../paper-2-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
