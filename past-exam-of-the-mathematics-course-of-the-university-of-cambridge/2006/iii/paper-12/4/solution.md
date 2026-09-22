<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The uniform modular [Frankl-Wilson theorem](../../../../../frankl-wilson-theorem.md) states the following. Let $p$ be prime, let $L\subseteq\mathbb F_p$ have size $s$, and let $\mathcal F$ be a rank-$k$ family on $[N]$, with $0\le s\le\min\{k,N-k\}$. Assume $k\bmod p\notin L$ and $|A\cap B|\bmod p\in L$ for every distinct $A,B\in\mathcal F$. Then

$$
\boxed{|\mathcal F|\le\binom Ns.}
$$

The restrictions concern distinct pairs; the diagonal size residue is explicitly excluded from $L$.

For each member $A$, over $\mathbb F_p$ form the [intersection polynomial](../../../../../intersection-polynomial.md)

$$
f_A(z_1,\ldots,z_N)=\prod_{\ell\in L}\left(\sum_{i\in A}z_i-\ell\right).
$$

At the characteristic vector $1_B$, its value vanishes when $B\ne A$ and is nonzero when $B=A$. Thus these functions are [linearly independent](../../../../../linear-independence.md) on the whole rank-$k$ layer: evaluate any linear relation at each family member in turn. Replacing every positive power of $z_i$ by $z_i$ preserves all Boolean evaluations, so the functions are restrictions of [multilinear polynomials](../../../../../multilinear-polynomial.md) of degree at most $s$.

We need the sharp [low-degree evaluation rank on a uniform layer](../../../../../low-degree-evaluation-rank-on-a-uniform-layer.md), not the larger whole-cube dimension $\sum_{j\le s}\binom Nj$. Let $M$ be the integer incidence [matrix](../../../../../matrix.md) with rows indexed by subsets $S$ of size at most $s$, columns by rank-$k$ sets $B$, and entries $1_{S\subseteq B}$. Over the rationals, if $|S|=j\le s$, then

$$
\sum_{\substack{S\subseteq T\subseteq[N]\\|T|=s}}M_{T,\cdot}
=\binom{k-j}{s-j}M_{S,\cdot}.
$$

This coefficient counts the possible $T$ inside each containing column set and is positive because $s\le k$. Consequently the degree-$s$ rows span all rows over $\mathbb Q$, giving rank at most $\binom Ns$. Every larger square minor is therefore the integer zero. Reducing those minors modulo $p$ shows the rank over $\mathbb F_p$ is also at most $\binom Ns$. This transfer avoids dividing by a [binomial coefficient](../../../../../binomial-coefficient.md) that might vanish modulo $p$. The independent functions $f_A$ lie in this row space, so their number is at most its rank. This proves the theorem in full.

For the requested forbidden-intersection application, split $\mathcal A$ into sets containing coordinate one and sets avoiding it. In the first part, delete one. Distinct original sets have intersection size between one and $2p-1$, excluding $p$. Their reduced intersections therefore lie between zero and $2p-2$, excluding $p-1$, so their residues belong to $L=\{0,\ldots,p-2\}$. The reduced set size is $2p-1$, whose residue is $p-1\notin L$. Frankl-Wilson on the ground set of size $4p-1$ bounds this part by $\binom{4p-1}{p-1}$.

For the avoiding part, first complement every set. The complements contain one, retain size $2p$, and satisfy

$$
|A^c\cap B^c|=4p-|A\cup B|=|A\cap B|.
$$

Delete one and apply the same argument. The [complement splitting for forbidden midpoint intersections](../../../../../complement-splitting-for-forbidden-midpoint-intersections.md) yields the stronger bound

$$
\boxed{|\mathcal A|\le2\binom{4p-1}{p-1}\le2\binom{4p}{p-1}.}
$$

The split is essential: a family may contain complementary pairs with intersection zero, preventing direct use of $L=\{1,\ldots,p-1\}$ on the original layer.

The [Borsuk conjecture](../../../../../borsuk-conjecture.md) asserted that a bounded subset of $\mathbb R^d$ of positive [diameter](../../../../../diameter.md) can be partitioned into $d+1$ subsets of strictly smaller [diameter](../../../../../diameter.md). Here is the [Kahn-Kalai counterexample to the Borsuk conjecture](../../../../../kahn-kalai-counterexample-to-the-borsuk-conjecture.md), implemented by balanced cut vectors. For each $X\in[4p]^{(2p)}$, define $v_X\in\mathbb R^{\binom{4p}{2}}$ whose coordinate indexed by an unordered pair $\{i,j\}$ is one when exactly one endpoint lies in $X$, and zero otherwise. Complementary sets give the same cut. Choose the representative with $1\in X$, obtaining exactly

$$
M=\binom{4p-1}{2p-1}
$$

distinct points: a cut determines its two parts, and fixing the side containing one removes its only ambiguity. Every cut has $(2p)^2=4p^2$ occupied coordinates, so all points lie in the [affine hyperplane](../../../../../affine-hyperplane.md) with coordinate sum $4p^2$. Its dimension is

$$
d=\binom{4p}{2}-1.
$$

We can identify this hyperplane isometrically with $\mathbb R^d$; no claim of full [affine span](../../../../../affine-hull.md) is needed.

For two side sets with $t=|X\cap Y|$, their [symmetric difference](../../../../../symmetric-difference.md) has $4p-2t$ points. The two cuts disagree exactly on pairs with one endpoint in that [symmetric difference](../../../../../symmetric-difference.md), giving the [balanced cut-vector distance formula](../../../../../balanced-cut-vector-distance-formula.md)

$$
\boxed{\|v_X-v_Y\|_2^2=(4p-2t)(2t)=4t(2p-t)
=4\bigl(p^2-(t-p)^2\bigr).}
$$

The [diameter](../../../../../diameter.md) is $2p$, attained exactly when $t=p$; such pairs exist even among representatives containing one. Thus a smaller-diameter part contains no pair with side intersection $p$. Since all representative sets already contain one, deleting that common coordinate and applying the preceding Frankl-Wilson argument bounds each part by $\binom{4p-1}{p-1}$. There is no extra factor two at this step. This is the cut construction described in [the original Kahn-Kalai paper](https://arxiv.org/abs/math/9307229); the distance and part-size calculations above give the required justification directly.

An explicit choice is $p=13$. The point set lies in dimension

$$
\boxed{d=\binom{52}{2}-1=1325.}
$$

The exact counts are

$$
M=\binom{51}{25}=247959266474052,\qquad
B=\binom{51}{12}=158753389900.
$$

Their ratio requires at least $\lceil M/B\rceil=1562$ smaller-diameter parts, exceeding $d+1=1326$. In particular,

$$
M-1326B=37452271466652>0.
$$

Rescaling the point set to [diameter](../../../../../diameter.md) one changes none of these partition counts. Therefore the [Borsuk counterexample in dimension 1325](../../../../../borsuk-counterexample-in-dimension-1325.md) is fully explicit. This is a concrete dimension, not a claim that it is the smallest possible counterexample dimension.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 12](../../paper-12-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
