<h1 id="6/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $q=1-p_0$. In [one-independent bond percolation](../../../../../../one-independent-bond-percolation.md), bond states in two sets with disjoint endpoint sets are independent as collections. In particular, the states of any finite [matching in a graph](../../../../../../matching-graph-theory.md) are mutually independent, by induction on its size. Neither translation invariance nor the [Harris lemma](../../../../../../harris-inequality.md) is assumed for this law.

If the origin's open cluster is finite, the outer boundary of the union of its vertex-centered unit squares contains a closed dual circuit surrounding the origin. A specified circuit of length $\ell$ corresponds to $\ell$ distinct closed primal bonds. Partition those bonds into four [matchings in a graph](../../../../../../matching-graph-theory.md): horizontal bonds according to the parity of the left endpoint's horizontal coordinate, and vertical bonds according to the parity of the lower endpoint's vertical coordinate. Some class has at least $\ell/4$ bonds. Their mutual independence and their individual closed probabilities at most $q$ imply

$$
\widetilde{\mathbb P}(\text{all circuit bonds closed})\leq q^{\ell/4}.
$$

This is the [Peierls circuit bound for one-independent percolation](../../../../../../peierls-circuit-bound-for-one-independent-percolation.md).

There are at most $4\ell3^\ell$ dual circuits of length $\ell$ enclosing the origin. To obtain this crude bound, choose a crossing of the positive horizontal ray; its distance from the origin is at most $\ell$, since the circuit also extends to the other side of the origin. There are at most $\ell$ choices for its dual edge, at most two orientations, and at most three choices at each subsequent step of a nonbacktracking walk. The stated bound allows extra slack and overcounting. The [union bound](../../../../../../boole-s-inequality.md) now gives

$$
\widetilde{\mathbb P}(|C_0|<\infty)\leq4\sum_{\ell\geq4}\ell(3q^{1/4})^\ell.
$$

For instance choose **$p_0=1-10^{-8}<1$**, so $x=3q^{1/4}=0.03$. The exact sum is

$$
4\sum_{\ell\geq4}\ell x^\ell=\frac{4x^4(4-3x)}{(1-x)^2}<1.
$$

It follows that **$\widetilde{\mathbb P}(|C_0|=\infty)>0$**. This deliberately nonoptimal constant suffices for existence of a universal $p_0$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [6](../../6.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
