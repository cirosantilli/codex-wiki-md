<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

The [Weak Hilbert Nullstellensatz](../../../../../weak-hilbert-nullstellensatz.md) states that if $k$ is an [algebraically closed field](../../../../../algebraically-closed-field.md), every [maximal ideal](../../../../../maximal-ideal.md) of $k[Y_1,\ldots,Y_s]$ is

$$
\boxed{(Y_1-a_1,\ldots,Y_s-a_s)\quad\text{for a unique }(a_1,\ldots,a_s)\in k^s.}
$$

Equivalently, every proper [ideal](../../../../../ideal.md) has a common zero. We prove the more general field statement, the [Zariski lemma](../../../../../zariski-s-lemma.md): a [field](../../../../../field.md) finitely generated as a $k$-[algebra](../../../../../algebra-split.md) is a [finite field extension](../../../../../finite-field-extension.md) of $k$.

Write such a field as $L=k[b_1,\ldots,b_s]$. Choose a maximal set of [algebraically independent elements](../../../../../algebraically-independent-elements.md) $t_1,\ldots,t_r$ among these generators and denote the remaining generators by $c_1,\ldots,c_h$. Each $c_j$ is an [algebraic element](../../../../../algebraic-element.md) over $K=k(t_1,\ldots,t_r)$, so $L/K$ is a [finite field extension](../../../../../finite-field-extension.md). Clearing the denominators in their monic equations, choose a nonzero $d\in k[t_1,\ldots,t_r]$ such that each $c_j$ is an [integral element](../../../../../integral-element.md) over

$$
D=k[t_1,\ldots,t_r,d^{-1}].
$$

Because $L$ is a field and $d^{-1}\in L$, we have $L=D[c_1,\ldots,c_h]$. Thus $L$ is an [integral extension](../../../../../integral-extension.md) of $D$.

A subring over which a field is integral must itself be a field. Indeed, for $0\ne a\in D$, an integral equation for $a^{-1}$ multiplied by $a^{m-1}$ expresses $a^{-1}$ as an element of $D$. But if $r>0$, the ring $D$ is not a field: choose an [irreducible polynomial](../../../../../irreducible-polynomial.md) $q(t_1)\in k[t_1]$ which does not divide $d$. There are infinitely many monic [irreducible polynomials](../../../../../irreducible-polynomial.md) in $k[t_1]$, by the usual product-plus-one argument, whereas only finitely many can divide the nonzero $d$. The [prime ideal](../../../../../prime-ideal.md) $(q)$ stays proper after inverting $d$, so $q$ has no inverse in $D$. Therefore $r=0$, proving that $L/k$ is a [finite field extension](../../../../../finite-field-extension.md), and in particular an [algebraic field extension](../../../../../algebraic-extension.md).

Apply the [Zariski lemma](../../../../../zariski-s-lemma.md) to the [residue field](../../../../../residue-field.md) $k[Y_1,\ldots,Y_s]/\mathfrak m$ of a [maximal ideal](../../../../../maximal-ideal.md). When $k$ is an [algebraically closed field](../../../../../algebraically-closed-field.md), this field is $k$ itself. The images $a_i$ of $Y_i$ then give $\mathfrak m=(Y_1-a_1,\ldots,Y_s-a_s)$, proving the [Weak Hilbert Nullstellensatz](../../../../../weak-hilbert-nullstellensatz.md).

For the real [Laurent polynomial ring](../../../../../laurent-polynomial-ring.md), the same argument applies because it is the [finitely generated algebra](../../../../../finitely-generated-algebra.md)

$$
R\cong\mathbb R[U_1,V_1,U_2,V_2]/(U_1V_1-1,U_2V_2-1).
$$

Every [residue field](../../../../../residue-field.md) at a [maximal ideal](../../../../../maximal-ideal.md) is consequently a [finite field extension](../../../../../finite-field-extension.md) of $\mathbb R$, and so is $\mathbb R$ or $\mathbb C$. Here we use the [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md), which makes $\mathbb C$ the [algebraic closure](../../../../../algebraic-closure.md) of $\mathbb R$ of degree two. The images of $X_1,X_2$ must be nonzero since these elements are [units](../../../../../unit-in-a-ring.md). It follows that the answer is

$$
\boxed{\mathfrak m_{\alpha,\beta}=\{f\in R:f(\alpha,\beta)=0\},\quad (\alpha,\beta)\in(\mathbb C^\times)^2,}
$$

with $(\alpha,\beta)$ and $(\overline\alpha,\overline\beta)$ defining the same [maximal ideal](../../../../../maximal-ideal.md). If both coordinates are real, evaluation has image $\mathbb R$; otherwise its image is $\mathbb C$. Thus every displayed [kernel](../../../../../kernel-of-a-linear-map.md) is maximal, and the [Zariski lemma](../../../../../zariski-s-lemma.md) shows that this list is exhaustive.

For explicit [generating sets of an ideal](../../../../../generating-set-of-an-ideal.md), there are three cases. For real nonzero $a,b$,

$$
\mathfrak m_{a,b}=(X_1-a,X_2-b).
$$

If $\alpha=a\in\mathbb R^\times$ and $\beta=s+it$ with $t\ne0$,

$$
\mathfrak m_{a,\beta}=(X_1-a,\ X_2^2-2sX_2+s^2+t^2).
$$

If $\alpha=u+iv$ with $v\ne0$ and $\beta=s+it$, then

$$
\mathfrak m_{\alpha,\beta}=\left(X_1^2-2uX_1+u^2+v^2,\ X_2-s-\frac{t}{v}(X_1-u)\right).
$$

The last two quotients are $\mathbb C$; the nonzero coordinate condition ensures that the Laurent inverses exist in them. There are no further coincidences in the classification: equal [kernels](../../../../../kernel-of-a-linear-map.md) induce an $\mathbb R$-[isomorphism](../../../../../isomorphism.md) between the evaluation image fields. The only $\mathbb R$-[automorphisms](../../../../../automorphism.md) of $\mathbb C$ are the identity and [complex conjugation](../../../../../complex-conjugation.md), so the two pairs must agree or be conjugate.

To prove the intersection assertion, fix a [prime ideal](../../../../../prime-ideal.md) $P$ and an element $f\notin P$. The [integral domain](../../../../../integral-domain.md) $B=R/P$ has nonzero image $\bar f$. Its [localization of a ring](../../../../../localization-of-a-ring.md) $B[\bar f^{-1}]$ is nonzero and still a [finitely generated algebra](../../../../../finitely-generated-algebra.md) over $\mathbb R$, so it has a [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak n$. By the [Zariski lemma](../../../../../zariski-s-lemma.md), the field $L=B[\bar f^{-1}]/\mathfrak n$ is finite over $\mathbb R$.

The image of $B$ in $L$ is a subring containing $\mathbb R$ and is a finite-dimensional $\mathbb R$-[vector space](../../../../../vector-space-split.md). It is an [integral domain](../../../../../integral-domain.md), hence a field: multiplication by any nonzero element is an injective [linear map](../../../../../linear-map.md) of a finite-dimensional [vector space](../../../../../vector-space-split.md) and therefore surjective. The [kernel](../../../../../kernel-of-a-linear-map.md) of $B\to L$ is thus a [maximal ideal](../../../../../maximal-ideal.md) which avoids $\bar f$, since $\bar f$ is invertible in $L$. Its inverse image in $R$ is a [maximal ideal](../../../../../maximal-ideal.md) containing $P$ but avoiding $f$. As this works for every $f\notin P$,

$$
\boxed{P=\bigcap_{\substack{\mathfrak m\supseteq P\\\mathfrak m\text{ maximal}}}\mathfrak m.}
$$

This is the [Jacobson ring](../../../../../jacobson-ring.md) property for this [Laurent polynomial ring](../../../../../laurent-polynomial-ring.md).

For a nonzero [finitely generated module](../../../../../finitely-generated-module.md) $M$, its set of [associated primes](../../../../../associated-prime-of-a-module.md) is

$$
\boxed{\operatorname{Ass}_R(M)=\{\operatorname{Ann}_R(m):0\ne m\in M,\ \operatorname{Ann}_R(m)\text{ is a prime ideal}\}.}
$$

Here $\operatorname{Ann}_R(m)=\{a\in R:am=0\}$ is the [annihilator](../../../../../annihilator-ring-theory.md) of the element. The [Laurent polynomial ring](../../../../../laurent-polynomial-ring.md) $R$ is a [Noetherian ring](../../../../../noetherian-ring.md), so the nonempty collection of [annihilators](../../../../../annihilator-ring-theory.md) of nonzero elements of $M$ has a maximal member, say $P=\operatorname{Ann}_R(m)$. It is proper because $m\ne0$.

If $ab\in P$ and $b\notin P$, then $bm\ne0$ and

$$
P\subseteq\operatorname{Ann}_R(bm),\qquad a\in\operatorname{Ann}_R(bm).
$$

Maximality forces $\operatorname{Ann}_R(bm)=P$, hence $a\in P$. Thus $P$ is a [prime ideal](../../../../../prime-ideal.md), proving $\boxed{\operatorname{Ass}_R(M)\ne\varnothing}$. This argument in fact only needs that $R$ is [Noetherian](../../../../../noetherian-ring.md), not the finite generation of $M$.

A proper [ideal](../../../../../ideal.md) $Q$ is $P$-[primary](../../../../../primary-ideal.md) when its [radical of an ideal](../../../../../radical-of-an-ideal.md) is $P$ and

$$
\boxed{ab\in Q,\ a\notin Q\ \Longrightarrow\ b^j\in Q\text{ for some }j\ge1.}
$$

Equivalently, $ab\in Q$ and $b\notin P$ imply $a\in Q$; equivalently, every [zero divisor](../../../../../zero-divisor.md) of $R/Q$ is [nilpotent](../../../../../nilpotent.md). These formulations distinguish the actual [primary ideal](../../../../../primary-ideal.md) property from the weaker assertion that there is only one [minimal prime ideal](../../../../../minimal-prime-ideal.md).

For the final example, set $u=X_1-1$ and $v=X_2-1$. Then

$$
\boxed{I=(u^2,uv),\qquad P=(u).}
$$

Since $R/P\cong\mathbb R[X_2,X_2^{-1}]$ is an [integral domain](../../../../../integral-domain.md), $P$ is a [prime ideal](../../../../../prime-ideal.md). Moreover $I\subseteq P$ and $u^2\in I$, so $\sqrt I=P$. Consequently $P$ is the unique [minimal prime ideal](../../../../../minimal-prime-ideal.md) over $I$.

Nevertheless $uv\in I$, while $u\notin I$ and no power of $v$ belongs to $I$. For the first assertion, reduce modulo $v$: the image of $I$ is $(u^2)$ in $\mathbb R[X_1,X_1^{-1}]$, and $u$ is not a multiple of $u^2$ because $u$ is a nonunit in this [integral domain](../../../../../integral-domain.md). For the second, $v\notin P$, so $v^j\notin P\supseteq I$ for every $j\ge1$. Thus $I$ is not a $P$-[primary ideal](../../../../../primary-ideal.md): a [unique minimal prime does not imply primary](../../../../../unique-minimal-prime-does-not-imply-primary.md). In $R/I$, the nonzero class of $u$ is killed by $v$, a [zero divisor](../../../../../zero-divisor.md) which is not [nilpotent](../../../../../nilpotent.md).

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 101](../../paper-101-split.md)
3. [Iii](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
