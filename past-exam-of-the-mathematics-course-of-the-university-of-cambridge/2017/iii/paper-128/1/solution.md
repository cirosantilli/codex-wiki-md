<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [Jacobson radical](../../../../../jacobson-radical.md) is $J(A)=\bigcap_L L$, where $L$ runs over the [maximal right ideals](../../../../../maximal-right-ideal.md) of $A$; equivalently, it is the intersection of the [annihilators](../../../../../annihilator-ring-theory.md) of all [simple modules](../../../../../irreducible-module.md). It is a two-sided [ideal](../../../../../ideal.md). A [projective module](../../../../../projective-module.md) has the lifting property against every surjective [R-module homomorphism](../../../../../module-homomorphism.md). A [finitely generated module](../../../../../finitely-generated-module.md) is a [projective module](../../../../../projective-module.md) precisely when it is a [direct summand](../../../../../direct-summand.md) of a finitely generated [free module](../../../../../free-module.md). An [indecomposable module](../../../../../indecomposable-module.md) is nonzero and admits no [direct sum](../../../../../direct-sum.md) decomposition into two nonzero [submodules](../../../../../submodule.md).

To calculate the [top of an indecomposable projective module](../../../../../top-of-an-indecomposable-projective-module.md), use the [right Artinian ring](../../../../../right-artinian-ring.md) hypothesis, namely the [descending chain condition](../../../../../descending-chain-condition.md) on [right ideals](../../../../../right-ideal.md). The [Hopkins-Levitzki theorem](../../../../../hopkins-levitzki-theorem.md) gives finite [composition length](../../../../../composition-length.md) of the right regular [module](../../../../../module-mathematics.md), hence of its [submodule](../../../../../submodule.md) $P$. Also $J=J(A)$ is a [nilpotent ideal](../../../../../nilpotent-ideal.md), and $A/J$ is a [semisimple ring](../../../../../semisimple-ring.md). Thus the [quotient module](../../../../../quotient-module.md) $\overline P=P/PJ$ is a [semisimple module](../../../../../semisimple-module.md); it is nonzero, since $P=PJ$ would imply $P=PJ^m=0$ for sufficiently large $m$.

Suppose $\overline P$ were not a [simple module](../../../../../irreducible-module.md). A nontrivial [direct sum](../../../../../direct-sum.md) decomposition of this [semisimple module](../../../../../semisimple-module.md) would give an [idempotent](../../../../../idempotent.md) $\alpha\in\operatorname{End}_A(\overline P)$ that is neither zero nor the identity. Writing $\pi:P\to\overline P$, the lifting property of the [projective module](../../../../../projective-module.md) $P$ gives $\beta\in\operatorname{End}_A(P)$ with $\pi\beta=\alpha\pi$. The [Fitting lemma](../../../../../fitting-lemma.md) for an [indecomposable module](../../../../../indecomposable-module.md) of finite [composition length](../../../../../composition-length.md) says that $\beta$ is either invertible or a [nilpotent element](../../../../../nilpotent.md). Its induced map $\alpha$ would then be invertible or a [nilpotent element](../../../../../nilpotent.md), respectively. Neither is possible for a nontrivial [idempotent](../../../../../idempotent.md). Therefore **$P/PJ(A)$ is simple**. This argument does not assume that an embedded [projective module](../../../../../projective-module.md) automatically splits off from the ambient [module](../../../../../module-mathematics.md).

A [block of an Artinian algebra](../../../../../block-of-an-artinian-algebra.md) is a nonzero two-sided [direct summand](../../../../../direct-summand.md) $Ae$ determined by a [primitive central idempotent](../../../../../primitive-central-idempotent.md) $e$: $e$ cannot be written as a sum of two nonzero orthogonal [central idempotents](../../../../../central-idempotent.md). Its identity is $e$. For a finite-dimensional [associative algebra](../../../../../associative-algebra-split.md), the [blocks of an Artinian algebra](../../../../../block-of-an-artinian-algebra.md) give its unique decomposition as a finite product of indecomposable [algebras](../../../../../algebra-split.md), or equivalently as a [direct sum](../../../../../direct-sum.md) of two-sided [ideals](../../../../../ideal.md).

For the [block of S3 in characteristic three](../../../../../block-of-s3-in-characteristic-three.md), put $A=kS_3$, $r=(123)$, $s=(12)$ and $a=r-1$. The [group algebra](../../../../../group-algebra.md) has [basis](../../../../../basis.md) $r^i,r^is$ for $0\leq i<3$. In [characteristic](../../../../../characteristic-of-a-field.md) three,

$$
a^3=0,\qquad sas=r^{-1}-1=-a+a^2.
$$

Consequently $I=aA$ is a two-sided [nilpotent ideal](../../../../../nilpotent-ideal.md), $I^3=0$, and $A/I\cong kC_2\cong k\times k$. A [nilpotent ideal](../../../../../nilpotent-ideal.md) lies in the [Jacobson radical](../../../../../jacobson-radical.md), and a quotient that is a [semisimple ring](../../../../../semisimple-ring.md) forces the reverse inclusion. Hence

$$
\boxed{J(A)=aA,\qquad \dim_k J(A)=4.}
$$

Define orthogonal [idempotents](../../../../../idempotent.md) $e_+=(1+s)/2$ and $e_-=(1-s)/2$. They sum to one, so the right regular [module](../../../../../module-mathematics.md) decomposes as

$$
\boxed{kS_3=e_+A\oplus e_-A,\qquad \dim_k e_+A=\dim_k e_-A=3.}
$$

The two summands are the [indecomposable projectives of S3 in characteristic three](../../../../../indecomposable-projectives-of-s3-in-characteristic-three.md). Each [direct summand](../../../../../direct-summand.md) is a [projective module](../../../../../projective-module.md), with [basis](../../../../../basis.md) $e_\pm,e_\pm r,e_\pm r^2$. Its [quotient module](../../../../../quotient-module.md) modulo multiplication by $J(A)$ is one-dimensional: the [trivial representation](../../../../../trivial-representation.md) for $e_+A$, and the [sign representation](../../../../../sign-representation.md) for $e_-A$. Each is an [indecomposable module](../../../../../indecomposable-module.md), since two nonzero [direct summands](../../../../../direct-summand.md) would each have nonzero [quotient module](../../../../../quotient-module.md) modulo $J(A)$, contradicting its one-dimensional top. For additional detail, the successive factors of the [radical series of a module](../../../../../radical-series-of-a-module.md) are the [trivial representation](../../../../../trivial-representation.md), [sign representation](../../../../../sign-representation.md), [trivial representation](../../../../../trivial-representation.md) for $e_+A$, and the [sign representation](../../../../../sign-representation.md), [trivial representation](../../../../../trivial-representation.md), [sign representation](../../../../../sign-representation.md) for $e_-A$. Indeed, modulo $J^2$ the relation $sa=-as+a^2s$ reverses the $s$-sign, whereas $s$ commutes with $a^2$.

The [center of an associative algebra](../../../../../center-of-an-associative-algebra.md) is spanned by the [conjugacy class](../../../../../conjugacy-class.md) sums $1$, $r+r^2$, and $(1+r+r^2)s$. Since $r+r^2=-1+a^2$ and $1+r+r^2=a^2$, this [center of an associative algebra](../../../../../center-of-an-associative-algebra.md) is

$$
Z(A)=k1\oplus ka^2\oplus ka^2s.
$$

Its [vector subspace](../../../../../vector-subspace.md) $ka^2\oplus ka^2s$ is a [square-zero ideal](../../../../../square-zero-ideal.md). If $d1+n$ is a [central idempotent](../../../../../central-idempotent.md), then $d^2=d$ and $(2d-1)n=0$. Thus $d=0$ or $1$ and $n=0$. There is no nontrivial [central idempotent](../../../../../central-idempotent.md), so **the whole group algebra is its single block**. The two three-dimensional [projective modules](../../../../../projective-module.md) above are a decomposition of the regular [module](../../../../../module-mathematics.md), not two [blocks of an Artinian algebra](../../../../../block-of-an-artinian-algebra.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 128](../../paper-128-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
