<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Gowers dichotomy theorem](../../../../../../gowers-dichotomy-theorem.md) states that **every infinite-dimensional Banach space contains either an unconditional basic sequence or a hereditarily indecomposable subspace**. Choose an initial [basic sequence](../../../../../../basic-sequence.md); it suffices to prove the result for its closed span $X$, with [basis constant](../../../../../../basis-constant.md) $K$.

We use the following precise finite-sequence form of the [Gowers Ramsey theorem for Banach spaces](../../../../../../gowers-ramsey-theorem-for-banach-spaces.md). Let $\mathcal A$ be an analytic family of finite normalized [block sequences](../../../../../../block-sequence.md), large in the sense that every infinite-dimensional [block subspace](../../../../../../block-subspace.md) contains a member. Given positive errors $\Delta=(\delta_i)$, some infinite-dimensional block subspace $Y$ makes $\mathcal A_\Delta$ strategically large. Here $\mathcal A_\Delta$ consists of tuples within $\delta_i$ coordinatewise of a member of $\mathcal A$. In the block game the subspace player chooses an infinite-dimensional block subspace at each turn; the vector player chooses a successive unit vector in it and can force a finite initial segment into $\mathcal A_\Delta$. This is the Ramsey theorem permitted without proof, not the dichotomy conclusion.

Assume $X$ contains no [unconditional basic sequence](../../../../../../unconditional-basic-sequence.md). For $\varepsilon>0$, let $\mathcal A_\varepsilon$ be the finite normalized block tuples $(x_1,\ldots,x_n)$ for which the odd and even spans contain unit vectors $u,v$ with $\|u-v\|<\varepsilon$. This family is analytic: in each finite length the witness coefficients and vectors range over finite-dimensional scalar spaces, and the strict distance test is continuous; taking a countable union of finite-support choices gives the block family.

It is large. Indeed, every block subspace has a conditional block basis, with coordinate projections of unbounded norms. Given a finite combination $z$, choose a set of coordinates $A$ with $\|P_Az\|$ arbitrarily large relative to $\|z\|$. Put $u_0=P_Az$, $v_0=-P_{A^c}z$. Then $u_0-v_0=z$ and $|\|u_0\|-\|v_0\||\leq\|z\|$, so

$$
\left\|\frac{u_0}{\|u_0\|}-\frac{v_0}{\|v_0\|}\right\|\leq\frac{2\|z\|}{\|u_0\|}.
$$

Group consecutive nonzero terms belonging to the same side into a single block, and normalize each group. The groups alternate between the two sides, and their odd and even spans contain these two normalized vectors. Interchanging their names if necessary gives a member of $\mathcal A_\varepsilon$.

Choose $\Delta$ with $8K\sum_i\delta_i<\varepsilon$. A game tuple in $\mathcal A_{\varepsilon,\Delta}$ actually belongs to $\mathcal A_{2\varepsilon}$. To check the perturbation explicitly, each coefficient of a unit vector in a normalized block tuple is bounded by $2K$. Replacing its coordinates by their nearby game vectors changes it by at most $2K\sum\delta_i$. Normalizing again changes the vector by at most twice that amount. Doing this for the two witnesses adds at most $8K\sum\delta_i$ to their distance.

The Ramsey theorem thus supplies a block subspace on which the vector player can force odd and even spans to contain unit vectors within $2\varepsilon$. Given any two infinite-dimensional block subspaces $U,V$ of that space, let the subspace player choose them alternately, using their successive tails to satisfy support order. The strategy produces the odd vectors in $U$ and the even vectors in $V$, so these subspaces contain the required nearby unit vectors.

Repeat inside decreasing block subspaces $Y_n$ with $\varepsilon_n\downarrow0$, and choose a diagonal normalized block sequence $(z_n)$ with $z_n\in Y_n$. Its tail from $n$ onward lies in $Y_n$. In $Z=[z_n]$, any two infinite-dimensional block subspaces can be restricted to this tail, hence contain unit vectors at distance less than $2\varepsilon_n$ for every $n$.

Finally this zero-angle statement extends to arbitrary infinite-dimensional closed subspaces $U,V$ of $Z$. Choose unit vectors in each subspace annihilating the first successively many basis coordinates, and approximate them by finite successive blocks with summably small errors. The coordinate bound $2K$ makes the resulting map from the block span to the original subspace arbitrarily close to the identity in operator norm. Apply the block-subspace zero-angle result and normalize the transported vectors; their added error can be made arbitrarily small. Thus the unit spheres of $U,V$ have distance zero.

By the equivalence proved in part (a), **$Z$ is hereditarily indecomposable**. This proves the dichotomy, including the passage from block subspaces to all subspaces.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 11](../../../paper-11-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
