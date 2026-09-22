<h1 id="9e/solution">Solution</h1>

↑ **Parent:** [9E](../9e.md)

A [Sylow subgroup](../../../../../sylow-subgroup.md) of a [finite group](../../../../../finite-group.md) $G$ is a subgroup whose order is the largest [power of a prime](../../../../../prime-power.md) $p$ dividing $|G|$. The [Sylow theorems](../../../../../sylow-theorems.md) say that such subgroups exist, that every $p$-subgroup lies in one, that all Sylow $p$-subgroups are conjugate, and that their number $n_p$ divides $|G|/p^a$ and obeys $n_p\equiv1\pmod p$.

For the last congruence, let one Sylow $p$-subgroup $P$ act by conjugation on the set of all Sylow $p$-subgroups. Every [orbit](../../../../../orbit-of-a-group-action.md) other than a fixed point has size divisible by $p$. If $Q$ is fixed, then $P,Q\leq N_G(Q)$. They are Sylow subgroups of this [normalizer](../../../../../normalizer.md), so they are conjugate within $N_G(Q)$; because every element of $N_G(Q)$ fixes $Q$ under conjugation, this forces $P=Q$. Thus there is exactly one fixed point and $n_p\equiv1\pmod p$.

Now let $H<A_n$ have [index](../../../../../index-of-a-subgroup.md) $m$ with $1<m<n$. The [coset action](../../../../../coset-action.md) gives a homomorphism

$$
A_n\longrightarrow S_m.
$$

Its [kernel](../../../../../kernel-of-a-group-homomorphism.md) is a [normal subgroup](../../../../../normal-subgroup.md) of the [simple group](../../../../../simple-group.md) $A_n$. It cannot be all of $A_n$, since the action is transitive and nontrivial, so it is trivial. This would embed $A_n$ into $S_m$, contrary to $|A_n|=n!/2>m!=|S_m|$. Hence no such subgroup exists.

Suppose finally that a group $G$ of order $90$ were simple. The Sylow count satisfies

$$
n_5\mid18,\qquad n_5\equiv1\pmod5,
$$

and simplicity excludes $n_5=1$, so $n_5=6$. Conjugation on these six subgroups gives a nontrivial homomorphism $G\to S_6$, which simplicity makes injective. Its image lies in $A_6$, because the composite with the [sign homomorphism](../../../../../sign-homomorphism.md) $S_6\to\{\pm1\}$ must be trivial. It would therefore be a subgroup of $A_6$ of index $360/90=4$, contradicting the result just proved. Thus

$$
\boxed{\text{no group of order }90\text{ is simple}.}
$$

## ↑ Ancestors (10)

1. [9E](../9e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
