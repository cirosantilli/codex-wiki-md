<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The [Rosenthal l1 theorem](../../../../../rosenthal-l1-theorem.md) states that **every bounded sequence in a real or complex Banach space has either a weakly Cauchy subsequence or a subsequence equivalent to the unit vector basis of $\ell^1$**. Equivalence means that there are $0<c\leq C<\infty$ such that $c\sum|a_i|\leq\|\sum a_ix_{n_i}\|\leq C\sum|a_i|$ for every finite scalar combination.

We use the infinite Ramsey result that every closed subset of $[\mathbb N]^\omega$ is a [Ramsey set of infinite subsets](../../../../../ramsey-set-of-infinite-subsets.md). It follows by taking complements in the open-set theorem proved in Question 6(a), and is also among the infinite Ramsey results permitted here.

Let $E$ be the closed span of the sequence and $K=B_{E^*}$ with its [weak-star topology](../../../../../weak-star-topology.md). It is compact by the [Banach-Alaoglu theorem](../../../../../banach-alaoglu-theorem.md). The functions $f_n(\phi)=\phi(x_n)$ are continuous and uniformly bounded. Pointwise convergence of a subsequence on $K$ is precisely the weakly Cauchy conclusion.

Choose a countable collection of pairs $(Q_0,Q_1)$ of disjoint closed rational boxes in the scalar plane, or intervals for real scalars. Write $u,v$ for their centres, $d=|u-v|>0$, and require their diameters to be at most some $\eta<d/(4\pi)$. Include arbitrarily small such boxes, so any two distinct scalar cluster points lie in the interiors of one such pair. For a fixed pair, say an infinite set $M$ oscillates if some $\phi\in K$ has $f_n(\phi)\in Q_0$ and $f_n(\phi)\in Q_1$ each for infinitely many $n\in M$.

There are two possibilities. If at some pair and some infinite $M$ every infinite subset oscillates, retain them. Otherwise enumerate the box pairs and successively thin so that no point oscillates for the current pair. A diagonal subsequence is eventually in each refined set, so has no point oscillating for any pair. A bounded scalar sequence with two cluster points would oscillate for a pair of boxes enclosing those points. Hence every scalar evaluation on that subsequence converges, giving the weakly Cauchy alternative.

In the remaining case put $A_n=f_n^{-1}(Q_0)$ and $B_n=f_n^{-1}(Q_1)$, closed subsets of $K$. Consider

$$
\mathcal C=\{(n_i)\in[M]^\omega:\bigcap_{i\text{ odd}}A_{n_i}\cap\bigcap_{i\text{ even}}B_{n_i}\ne\varnothing\}.
$$

This is closed. If the infinite intersection is empty, compactness gives an empty finite intersection, and every infinite sequence with the same sufficiently long initial segment also has an empty intersection. The complement is therefore open. Apply closed-set Ramsey to obtain an infinite $L\subseteq M$ homogeneous for $\mathcal C$.

It cannot be homogeneous outside $\mathcal C$: the retained oscillation property provides a point visiting both level sets infinitely often on $L$, from which we can select an alternating sequence belonging to $\mathcal C$. Thus every infinite subset of $L$ is in $\mathcal C$.

Pass to the even-indexed members $L'=(l_2,l_4,\ldots)$. The pairs $(A_n,B_n)$ for $n\in L'$ are independent: every assignment of either $A$ or $B$ to finitely many chosen indices has a common point. Indeed insert zero or one unused members of $L$ before and between the specified indices to arrange their required odd or even positions, then complete to an infinite sequence. The gaps between even-indexed members supply these spare indices. Membership of that infinite sequence in $\mathcal C$ supplies the point realizing the finite assignment.

Take any finite complex coefficients $a_i$. Some unit scalar $\zeta$ satisfies

$$
\sum_i|\operatorname{Re}(\zeta a_i)|\geq\frac2\pi\sum_i|a_i|,
$$

because the average over the unit circle is exactly the right side. Put $\varepsilon_i=\operatorname{sign}\operatorname{Re}(\zeta a_i)$, choosing either sign at zero. Independence supplies functionals $\phi,\psi\in K$ such that $f_{n_i}(\phi)$ lies near $u$ and $f_{n_i}(\psi)$ near $v$ when $\varepsilon_i=1$, with the assignments reversed when $\varepsilon_i=-1$. Thus

$$
\left|(\phi-\psi)\left(\sum_i a_ix_{n_i}\right)-(u-v)\sum_i\varepsilon_i a_i\right|\leq2\eta\sum_i|a_i|.
$$

Also $|\sum\varepsilon_i a_i|\geq\sum|\operatorname{Re}(\zeta a_i)|$. Since $\|\phi-\psi\|\leq2$, we conclude

$$
\boxed{\left\|\sum_i a_ix_{n_i}\right\|\geq\left(\frac d\pi-\eta\right)\sum_i|a_i|.}
$$

The coefficient is positive by the box choice, and boundedness of the original sequence gives the upper estimate. This proves the $\ell^1$ alternative over complex scalars. For real scalars simply partition by the signs of the coefficients; the same calculation works and gives the stronger lower constant $d/2-\eta$. This completes the proof.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 11](../../paper-11-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
