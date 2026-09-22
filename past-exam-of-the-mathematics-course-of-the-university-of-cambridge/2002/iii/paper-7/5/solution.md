<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [representation of a Banach algebra](../../../../../representation-of-a-banach-algebra.md) is a complex-linear multiplicative map $\pi:A\to\operatorname{End}_{\mathbb C}(X)$. A nonzero irreducible action of a [unital algebra](../../../../../unital-algebra.md) automatically has $\pi(1)=I$: the image of the idempotent $\pi(1)$ is a nonzero invariant subspace and hence is all of $X$. An [algebraically irreducible representation of a Banach algebra](../../../../../algebraically-irreducible-representation-of-a-banach-algebra.md) is a nonzero action if it has no nonzero proper [invariant submodule](../../../../../invariant-submodule.md), whether [closed](../../../../../closed-set.md) or not. A [normed representation of a Banach algebra](../../../../../normed-representation-of-a-banach-algebra.md) has $\pi(a)$ bounded for each $a$ on a preassigned [normed vector space](../../../../../normed-vector-space.md) $X$; [continuity](../../../../../continuous-function.md) of $\pi$ as an operator-norm-valued map is a further conclusion. This must not be confused with topological irreducibility, which excludes only [closed](../../../../../closed-set.md) [invariant subspaces](../../../../../invariant-subspace.md). Unitizing the algebra extends a nonunital action by $\pi(a+\lambda1)=\pi(a)+\lambda I$, so it is enough to discuss the [unital](../../../../../unital-algebra.md) case.

For $\xi\ne0$, irreducibility gives $A\xi=X$. The annihilator $L_\xi=\{a:\pi(a)\xi=0\}$ is a [maximal left ideal](../../../../../maximal-left-ideal.md): an intermediate [left ideal](../../../../../left-ideal.md) gives an intermediate [submodule](../../../../../submodule.md) of $X$. It is [closed](../../../../../closed-set.md) by the Neumann-series argument for [maximal left ideals](../../../../../maximal-left-ideal.md). Consequently $A/L_\xi$ transports a complete quotient [norm](../../../../../norm.md) to $X$, and left multiplication is contractive in this [norm](../../../../../norm.md). Every [algebraically irreducible representation of a Banach algebra](../../../../../algebraically-irreducible-representation-of-a-banach-algebra.md) can therefore be realized continuously on a [Banach space](../../../../../banach-space-split.md). This alone does not prove [continuity](../../../../../continuous-function.md) for its preassigned [norm](../../../../../norm.md).

The kernel of $\pi$ is the intersection of the [closed](../../../../../closed-set.md) [left ideals](../../../../../left-ideal.md) $L_\xi$ and is a [closed](../../../../../closed-set.md) [primitive ideal](../../../../../primitive-ideal.md). The [Jacobson radical](../../../../../jacobson-radical.md) is the intersection of all [primitive ideals](../../../../../primitive-ideal.md), equivalently the intersection of [maximal left ideals](../../../../../maximal-left-ideal.md). Thus these quotient representations detect semisimplicity. Equivalent [algebra representations](../../../../../representation-of-an-associative-algebra.md) are related by a bijective [module homomorphism](../../../../../module-homomorphism.md).

The algebra of [module endomorphisms](../../../../../module-endomorphism.md) is exactly $\mathbb C I$. Indeed, if a [module endomorphism](../../../../../module-endomorphism.md) $D$ sends a fixed cyclic [vector](../../../../../vector.md) $\xi$ to $a\xi$, then $D(b\xi)=ba\xi$. It is induced by bounded right multiplication by $a$ on $A/L_\xi$, so is bounded for the [quotient norm on an irreducible Banach module](../../../../../quotient-norm-on-an-irreducible-banach-module.md). Every nonzero [module endomorphism](../../../../../module-endomorphism.md) is injective and surjective by irreducibility, and its inverse is bounded by the same argument. This [commutant of an operator algebra](../../../../../commutant-of-an-operator-algebra.md) is a [closed](../../../../../closed-set.md) division [subalgebra](../../../../../subalgebra.md) of the [bounded operators](../../../../../continuous-linear-operator.md) on this Banach module; the [Gelfand-Mazur theorem](../../../../../gelfand-mazur-theorem.md) makes it $\mathbb C I$.

The [Jacobson density theorem](../../../../../jacobson-density-theorem.md) now says that for finitely many [linearly independent](../../../../../linear-independence.md) $\xi_1,\ldots,\xi_n$ and arbitrary $\eta_1,\ldots,\eta_n$, one element of $A$ sends all $\xi_j$ to $\eta_j$. Here is the induction behind it. The one-vector assertion is $A\xi_1=X$. Assuming the first $n-1$ coordinates can be prescribed, set $L=\{a:a\xi_j=0\ (j<n)\}$. Its image $L\xi_n$ is an [invariant subspace](../../../../../invariant-subspace.md). If it is $X$, it adjusts the last image without changing the first ones. If it is zero, the rule $(a\xi_1,\ldots,a\xi_{n-1})\mapsto a\xi_n$ is a well-defined module map $X^{n-1}\to X$. Each coordinate map is scalar by the [module endomorphism](../../../../../module-endomorphism.md) result, forcing $\xi_n$ to be a [linear combination](../../../../../linear-combination.md) of the earlier [vectors](../../../../../vector.md), a contradiction. This proves the assertion.

We can now give Johnson's [continuity](../../../../../continuous-function.md) argument with its crucial construction. If $X$ is finite dimensional, the [closed](../../../../../closed-set.md) kernel has finite codimension and $A/\ker\pi$ is finite dimensional, so $\pi$ is [continuous](../../../../../continuous-function.md). Suppose instead that $X$ is infinite dimensional. Let

$$
Y=\{\xi\in X:a\mapsto\pi(a)\xi\text{ is continuous}\}.
$$

This is an [invariant submodule](../../../../../invariant-submodule.md), because the orbit map of $\pi(b)\xi$ is the orbit map of $\xi$ composed with the bounded map $a\mapsto ab$. Thus either $Y=X$ or $Y=0$.

To rule out $Y=0$, choose [linearly independent](../../../../../linear-independence.md) unit [vectors](../../../../../vector.md) $\xi_0,\xi_1,\ldots$. There are elements $a_n\in A$ such that, with $c_n=a_n\cdots a_1$,

$$
\pi(c_m)\xi_n=0\quad(m>n),\qquad
\{\pi(c_n)\xi_j:j\ge n\}\text{ is linearly independent}.
$$

For completeness, construct them in the canonical quotient-norm Banach module. At stage $n$ the current tail [vectors](../../../../../vector.md) are independent. In the [closed](../../../../../closed-set.md) left annihilator of its first [vector](../../../../../vector.md), density permits arbitrary images of any finite list of the remaining [vectors](../../../../../vector.md). The condition that finitely many such images are independent is [open](../../../../../open-set.md) in this Banach subspace and dense: perturb any element by $t$ times an element prescribing independent images; a suitable determinant is a nonzero [polynomial](../../../../../polynomial-split.md) in $t$, with only finitely many exceptional values. The [Baire category theorem](../../../../../baire-category-theorem.md) intersects these [open](../../../../../open-set.md) dense conditions for all initial finite tail lists. The resulting $a_n$ kills the first current [vector](../../../../../vector.md) and retains independence of the entire remaining tail. This is the [countable annihilation sequence in an irreducible Banach module](../../../../../countable-annihilation-sequence-in-an-irreducible-banach-module.md).

The [gliding-hump continuity principle](../../../../../gliding-hump-continuity-principle.md) supplies the other ingredient: if $E,F$ are [Banach spaces](../../../../../banach-space-split.md), $S:E\to F$ is linear, $T_j:E\to E$ and $U_n:F\to F_n$ are bounded, and $U_nST_1\cdots T_m$ is [continuous](../../../../../continuous-function.md) whenever $m>n$, then $U_nST_1\cdots T_n$ is [continuous](../../../../../continuous-function.md) eventually. The product form of this principle is recorded in [Proposition 1.3 of Thomas's paper](https://msp.org/pjm/1993/159-1/pjm-v159-n1-p08-p.pdf). Here is the contradiction mechanism. Rescale so $\|T_j\|,\|U_n\|\le1$ and put $P_m=T_1\cdots T_m$. If infinitely many diagonal maps are discontinuous, choose increasing $n_j$ and successively tiny $x_j$ so

$$
\|U_{n_j}SP_{n_j}x_j\|>j+1+\sum_{i<j}\|U_{n_j}SP_{n_i}x_i\|.
$$

Also choose $\|x_j\|\le2^{-j}/(1+\max_{i<j}\|U_{n_i}SP_{n_i+1}\|)$. The convergent sum $x=\sum_jP_{n_j}x_j$ has, after its $j$th term, a tail factoring through $P_{n_j+1}$. Applying that [continuous](../../../../../continuous-function.md) composite bounds the tail contribution by one. The display forces $\|U_{n_j}Sx\|>j$, contradicting $\|U_{n_j}Sx\|\le\|Sx\|$. Only finite decompositions and the [continuous](../../../../../continuous-function.md) tail composites are used; no unjustified interchange of a discontinuous map with an infinite sum occurs.

Apply this principle with $E=A$, $F=\mathcal B(\overline X)$, where $\overline X$ is the completion in the original [norm](../../../../../norm.md), and $S(a)$ the bounded extension of $\pi(a)$. Set $T_j(a)=aa_j$ and $U_n(R)=R\xi_n$. Then

$$
U_nST_1\cdots T_m(a)=\pi(a)\pi(a_m\cdots a_1)\xi_n.
$$

For $m>n$ this is zero, hence [continuous](../../../../../continuous-function.md). For $m=n$ it is the orbit map of a nonzero [vector](../../../../../vector.md), hence discontinuous if $Y=0$. This contradicts the principle. Therefore $Y=X$.

Finally, apply the [Uniform boundedness principle](../../../../../uniform-boundedness-principle.md) on the [Banach space](../../../../../banach-space-split.md) $A$ to the [continuous](../../../../../continuous-function.md) maps $a\mapsto\pi(a)\xi$ indexed by $\|\xi\|\le1$. They are pointwise bounded because each individual $\pi(a)$ is bounded in the original [norm](../../../../../norm.md). It gives

$$
\boxed{\|\pi(a)\|\le C\|a\|\quad(a\in A).}
$$

This proves [Johnson's continuity theorem for irreducible normed representations](../../../../../johnson-s-continuity-theorem-for-irreducible-normed-representations.md), including when the original [normed vector space](../../../../../normed-vector-space.md) is incomplete. The quotient [norm](../../../../../norm.md), countable density construction, and gliding hump explain the substantive steps rather than assuming the desired [continuity](../../../../../continuous-function.md) in advance.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 7](../../paper-7-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
