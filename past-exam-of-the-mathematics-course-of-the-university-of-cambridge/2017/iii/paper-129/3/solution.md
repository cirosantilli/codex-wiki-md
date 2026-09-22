<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Work in positive dimension $n\geq1$. A [cap set](../../../../../cap-set.md) has no distinct zero-sum triple. Over the [finite field](../../../../../finite-field.md) $\mathbb F_3$, if two elements of a zero-sum triple agree then all three agree, since $2=-1$. Thus a zero-sum triple in a [cap set](../../../../../cap-set.md) must be diagonal. We prove the [Ellenberg–Gijswijt cap-set bound](../../../../../ellenberg-gijswijt-cap-set-bound.md) by the [polynomial method in combinatorics](../../../../../polynomial-method-in-combinatorics.md), keeping the exponential constant explicit and removing the fixed prefactor.

First prove the needed [slice rank of a diagonal tensor](../../../../../slice-rank-of-a-diagonal-tensor.md) over any [field](../../../../../field.md). The [slice rank](../../../../../slice-rank.md) of a three-variable [tensor](../../../../../tensor.md) is the least number of terms in a decomposition of the forms $a(x)b(y,z)$, $c(y)d(x,z)$, and $e(z)h(x,y)$. A [diagonal tensor](../../../../../diagonal-tensor.md) on a set of [cardinality](../../../../../cardinality.md) $m$, with every diagonal entry nonzero, has [slice rank](../../../../../slice-rank.md) at most $m$ by one slice for each entry. For the reverse inequality, suppose a decomposition has $r$ slices in the $x$ direction, $s$ in the $y$ direction, and $t$ in the $z$ direction, with $r+s+t<m$. Let

$$
W=\left\{u\in F^m:\sum_xu(x)a_i(x)=0\text{ for every }1\leq i\leq r\right\}.
$$

The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) gives $\dim W\geq m-r$. The [maximum-support vector in a finite-dimensional subspace](../../../../../maximum-support-vector-in-a-finite-dimensional-subspace.md) lemma supplies $u\in W$ with at least $m-r$ nonzero coordinates: choose $u$ of maximum [support of a vector](../../../../../support-of-a-vector.md); restriction $W\to F^{\operatorname{supp}u}$ must be injective, or adding a nonzero [kernel of a linear map](../../../../../kernel-of-a-linear-map.md) element would strictly enlarge that [support of a vector](../../../../../support-of-a-vector.md). This argument is valid over [finite fields](../../../../../finite-field.md), without any assumption that a generic vector avoids all coordinate hyperplanes.

Contract the proposed [tensor](../../../../../tensor.md) decomposition in $x$ against $u$. The [diagonal tensor](../../../../../diagonal-tensor.md) becomes a diagonal [matrix](../../../../../matrix.md) of [matrix rank](../../../../../matrix-rank.md) at least $m-r$. All $x$ slices vanish. Each remaining $y$ or $z$ slice becomes a [matrix](../../../../../matrix.md) of [matrix rank](../../../../../matrix-rank.md) at most one, so [subadditivity of matrix rank](../../../../../subadditivity-of-matrix-rank.md) gives [matrix rank](../../../../../matrix-rank.md) at most $s+t<m-r$, a contradiction. Therefore the [slice rank of a diagonal tensor](../../../../../slice-rank-of-a-diagonal-tensor.md) is exactly $m$.

Now, for a [cap set](../../../../../cap-set.md) $A\subseteq\mathbb F_3^n$, consider the [polynomial](../../../../../polynomial-split.md)

$$
P(x,y,z)=\prod_{i=1}^n\bigl(1-(x_i+y_i+z_i)^2\bigr).
$$

Each factor is one when its argument is zero and zero otherwise, because the two nonzero elements of $\mathbb F_3$ have square one. Thus $P$ is the [indicator function](../../../../../indicator-function.md) of $x+y+z=0$. Restricted to $A^3$, it is a [diagonal tensor](../../../../../diagonal-tensor.md) with every diagonal entry one, and its [slice rank](../../../../../slice-rank.md) is $|A|$.

Every [monomial](../../../../../monomial.md) in the expansion has individual exponents at most two and total [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $2n$. Consequently at least one of its $x$, $y$, or $z$ blocks has [polynomial degree](../../../../../degree-of-a-polynomial.md) at most $\lfloor2n/3\rfloor$. Assign each [monomial](../../../../../monomial.md) to one such block, breaking ties in a fixed way, and collect assigned terms by the [monomial](../../../../../monomial.md) in that block. Each collection is a slice. If

$$
m_n=\#\left\{a\in\{0,1,2\}^n:\sum_i a_i\leq\left\lfloor\frac{2n}{3}\right\rfloor\right\},
$$

there are at most $m_n$ slices in each direction. Thus $|A|\leq3m_n$.

The [low-degree monomial count for the cap-set bound](../../../../../low-degree-monomial-count-for-the-cap-set-bound.md) follows directly from a weighted sum. Each exponent vector counted by $m_n$ satisfies $1\leq2^{2n/3-\sum_i a_i}$, so

$$
m_n\leq2^{2n/3}\sum_{a\in\{0,1,2\}^n}2^{-\sum_i a_i}
=\left(\frac74\,2^{2/3}\right)^n=\theta^n.
$$

This supplies its own elementary exponential estimate; no unstated probabilistic estimate is required. Since $\theta^3=343/16<27$, we have $\theta<3$, but $|A|\leq3\theta^n$ alone would leave a fixed prefactor.

Use [Cartesian powers of cap sets](../../../../../cartesian-powers-of-cap-sets.md) to remove that prefactor. The $k$-fold [Cartesian product](../../../../../cartesian-product.md) $A^k\subseteq\mathbb F_3^{nk}$ is still a [cap set](../../../../../cap-set.md): in each block, a zero-sum triple of its elements must have all three entries equal. Hence $|A|^k\leq3\theta^{nk}$. Taking $k$th roots and letting $k$ tend to infinity proves the [removal of an exponential prefactor by Cartesian powers](../../../../../removal-of-an-exponential-prefactor-by-cartesian-powers.md):

$$
\boxed{|A|\leq\theta^n,\qquad\theta=\frac74\,2^{2/3}<\frac{14}{5}<3.}
$$

The strict middle inequality follows by cubing: $343/16<(14/5)^3$. We can therefore take

$$
\boxed{C=\frac{14}{5}.}
$$

For every $n\geq1$, a set with $|A|\geq C^n$ cannot be a [cap set](../../../../../cap-set.md), and hence contains the required distinct triple. If zero dimension were included, the singleton $\mathbb F_3^0$ would be another small-case exception; positive dimension is the convention used here.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 129](../../paper-129-split.md)
3. [Iii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
