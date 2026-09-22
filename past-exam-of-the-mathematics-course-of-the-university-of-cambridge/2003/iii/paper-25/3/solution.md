<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Write $e(t)=e^{2\pi it}$ and $N=n+1$. A convenient form of the [quadratic Weyl inequality](../../../../../quadratic-weyl-inequality.md) is the following: if $q\ge1$, $(a,q)=1$ and $|\alpha-a/q|\le q^{-2}$, then

$$
\boxed{\left|\sum_{x=0}^{N-1}e(\alpha x^2)\right|^2
\ll\left(\frac{N^2}{q}+N+q\right)\log(2q).}
$$

The implied constant is absolute. In particular the familiar square-root saving is $|S|\ll(N^2/q+N+q)^{1/2}\log(2q)^{1/2}$. We prove all estimates used in this statement.

First, the finite [geometric series](../../../../../geometric-series.md) identity gives

$$
\left|\sum_{x=0}^{L-1}e(\theta x)\right|
\le\min\left(L,\frac1{2\|\theta\|}\right),
$$

where $\|\theta\|$ denotes distance to the nearest integer and the second bound is interpreted as infinite when that distance is zero. Indeed the sum is $(1-e(L\theta))/(1-e(\theta))$, and $|1-e(\theta)|=2|\sin\pi\theta|\ge4\|\theta\|$. This proves the [exponential geometric sum bound](../../../../../exponential-geometric-sum-bound.md).

Expand the squared [quadratic exponential sum](../../../../../quadratic-exponential-sum.md) by the difference $h$ between its indices. Since $(x+h)^2-x^2=2hx+h^2$, the diagonal and the paired off-diagonals give

$$
|S|^2\le N+2\sum_{h=1}^{N-1}\min\left(N,\frac1{2\|2\alpha h\|}\right).
$$

For $q\ge16$, partition the $h$ into consecutive blocks of length at most $L=\lfloor q/8\rfloor$. Within one block, two distinct indices have difference $0<|d|<q/2$. Since the denominator of $2a/q$ after reduction is at least $q/2$, $\|2ad/q\|\ge1/q$. Therefore

$$
\|2\alpha d\|\ge\|2ad/q\|-2|d|\,|\alpha-a/q|
\ge\frac{3}{4q}.
$$

Thus the points $2\alpha h$ in a block are separated on the circle by at least $3/(4q)$.

For any such separated set, at most an absolute number of points lie in each pair of arcs whose distances from zero are between $j/(4q)$ and $(j+1)/(4q)$. The closest few contribute $O(N)$ to the capped reciprocal sum; the remaining arcs contribute $O(q/j)$ for $1\le j\le4q$. Summing the harmonic series, using $\sum_{j\le m}j^{-1}\le1+\log m$, proves a block bound $O(N+q\log(2q))$. This is the required [separated reciprocal-distance sum](../../../../../separated-reciprocal-distance-sum.md) estimate, with its proof supplied here. There are $O(N/q+1)$ blocks, so

$$
|S|^2\ll N+\left(\frac Nq+1\right)(N+q\log(2q))
\ll(N^2/q+N+q)\log(2q).
$$

For $q<16$, the trivial bound $|S|\le N$ already implies this estimate after increasing the absolute constant. This completes the proof, including the small denominators and the possible common factor of $2$ and $q$.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 25](../../paper-25-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
