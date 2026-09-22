<h1 id="6e/solution">Solution</h1>

↑ **Parent:** [6E](../6e.md)

For any [permutation](../../../../../permutation.md) $\tau$, conjugating a [permutation cycle](../../../../../permutation-cycle.md) relabels its entries:

$$
\tau(a_1\,a_2\,\ldots,a_r)\tau^{-1}=(\tau(a_1)\,\tau(a_2)\,\ldots,\tau(a_r)).
$$

Indeed, the conjugate sends $\tau(a_j)$ to $\tau(a_{j+1})$ and fixes the other relabeled entries exactly as the original [permutation cycle](../../../../../permutation-cycle.md) does. Therefore [conjugation](../../../../../conjugation.md) preserves the multiset of [permutation cycle](../../../../../permutation-cycle.md) lengths. Conversely, if two [permutations](../../../../../permutation.md) have the same [cycle type](../../../../../cycle-type.md), pair their [permutation cycles](../../../../../permutation-cycle.md) of each length and let $\tau$ carry the $j$th entry of each first [permutation cycle](../../../../../permutation-cycle.md) to the $j$th entry of its partner. Include one-cycles for fixed points. This defines a [bijection](../../../../../bijection.md) of all labels, and the displayed relabeling identity makes the [permutations](../../../../../permutation.md) conjugate. Thus

$$
\boxed{\sigma\sim_{S_n}\rho\quad\Longleftrightarrow\quad\sigma,\rho\text{ have the same cycle type}.}
$$

For $n\geq2$, the [alternating conjugacy class splitting criterion](../../../../../alternating-conjugacy-class-splitting-criterion.md) says that an even [permutation](../../../../../permutation.md) has the same class in $A_n$ and $S_n$ precisely when its type is not a collection of pairwise distinct odd lengths. Equivalently, **there is an even-length [permutation cycle](../../../../../permutation-cycle.md) or a repeated [permutation cycle](../../../../../permutation-cycle.md) length**, counting each fixed point as a length-one [permutation cycle](../../../../../permutation-cycle.md). Distinct odd lengths instead give two alternating-group classes. For $n=1$, $A_1=S_1$ and the sole class is the same; the index-two splitting criterion is not applicable.

Squaring an odd-length [permutation cycle](../../../../../permutation-cycle.md) keeps one [permutation cycle](../../../../../permutation-cycle.md) of that length, since advancing by two visits all of its entries. Squaring an even-length [permutation cycle](../../../../../permutation-cycle.md) splits it into two [permutation cycles](../../../../../permutation-cycle.md), each of half that length. Thus any even-length [permutation cycle](../../../../../permutation-cycle.md) strictly increases the total [permutation cycle](../../../../../permutation-cycle.md) count on squaring, while odd [permutation cycles](../../../../../permutation-cycle.md) leave that count unchanged. The [cycle type](../../../../../cycle-type.md) can agree with its square exactly when every length is odd. This proves [permutation conjugate to its square](../../../../../permutation-conjugate-to-its-square.md):

$$
\boxed{\sigma\sim_{S_n}\sigma^2\quad\Longleftrightarrow\quad\text{every cycle length is odd}
\quad\Longleftrightarrow\quad\operatorname{ord}(\sigma)\text{ is odd}.}
$$

The final equivalence follows because the [order of a group element](../../../../../order-of-a-group-element.md) that is a [permutation](../../../../../permutation.md) is the [least common multiple](../../../../../least-common-multiple.md) of its [permutation cycle](../../../../../permutation-cycle.md) lengths.

The possible even types on five labels are the identity, a three-cycle, a product of two disjoint [transpositions](../../../../../transposition-permutation.md) and a five-cycle. The identity and the double [transpositions](../../../../../transposition-permutation.md) are their own inverses. For a three-cycle $(a\,b\,c)$ with unused labels $d,e$, the even [permutation](../../../../../permutation.md) $(b\,c)(d\,e)$ conjugates it to its inverse. For a five-cycle $(a\,b\,c\,d\,e)$, the even [permutation](../../../../../permutation.md) $(b\,e)(c\,d)$ reverses its order. Therefore **every element of $A_5$ is conjugate to its inverse within $A_5$**. Inverting a five-cycle uses two [transpositions](../../../../../transposition-permutation.md), in agreement with [inversion of an odd cycle in an alternating group](../../../../../inversion-of-an-odd-cycle-in-an-alternating-group.md).

A small counterexample elsewhere is

$$
\boxed{n=3,\qquad\sigma=(1\,2\,3).}
$$

The [alternating group](../../../../../alternating-group.md) $A_3=\{e,(1\,2\,3),(1\,3\,2)\}$ is cyclic and therefore abelian. Every [conjugacy class](../../../../../conjugacy-class.md) in an [abelian group](../../../../../abelian-group.md) is a singleton, while $\sigma\ne\sigma^{-1}$. Thus these two elements are not conjugate in $A_3$.

## ↑ Ancestors (10)

1. [6E](../6e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
