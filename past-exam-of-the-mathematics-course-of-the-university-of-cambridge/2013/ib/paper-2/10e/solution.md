<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

A set is [linearly dependent](../../../../../linear-dependence.md) if some finite selection of distinct vectors admits a relation $\sum_jc_jv_j=0$ with coefficients not all zero. For a finite set this is just such a nontrivial relation using its vectors.

Prove dependence of $n+1$ vectors in $\mathbb R^n$ by induction, starting with the zero-dimensional case. If all first coordinates vanish, select $n$ of the vectors and apply induction in $\mathbb R^{n-1}$. Otherwise relabel so the last vector has first coordinate $a\ne0$. For $1\leq j\leq n$, put $w_j=v_j-(v_{j,1}/a)v_{n+1}$. These $n$ vectors have zero first coordinate, so induction supplies $\sum_{j=1}^nc_jw_j=0$, with some $c_j\ne0$. Expanding gives a nontrivial [linear dependence](../../../../../linear-dependence.md) among the original vectors. The same proof works over any [field](../../../../../field.md).

Now express vectors of $V$ in coordinates relative to its given $n$-element [basis](../../../../../basis.md). Any other [basis](../../../../../basis.md) has at most $n$ elements: more would contain $n+1$ [linearly dependent](../../../../../linear-dependence.md) vectors. If it has $m<n$ elements, expressing the original [basis](../../../../../basis.md) in its coordinates makes the original $n$ vectors [linearly dependent](../../../../../linear-dependence.md), a contradiction. Thus **every [basis](../../../../../basis.md) has exactly $n$ elements**.

Finally, the functions $\sin(jx)$, $j=1,2,\ldots$, are bounded and continuous. Any finite relation among them can be multiplied by $\sin(rx)$ and integrated over $[0,2\pi]$. The [orthogonality](../../../../../orthogonal-vectors.md) identity

$$
\int_0^{2\pi}\sin(jx)\sin(rx)\,dx=\pi\,\delta_{jr}
$$

forces every coefficient to vanish. Arbitrarily large [linearly independent](../../../../../linear-independence.md) finite sets exist, so **the [vector space](../../../../../vector-space-split.md) of bounded continuous functions is infinite-dimensional**.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
