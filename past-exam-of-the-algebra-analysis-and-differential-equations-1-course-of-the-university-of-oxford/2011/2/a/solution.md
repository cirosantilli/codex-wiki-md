<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Gram-Schmidt process](../../../../gram-schmidt-process.md) subtracts projections onto directions already constructed and then normalizes. Define recursively

$$
w_k=v_k-\sum_{j<k}\langle v_k,e_j\rangle e_j,\qquad e_k=\frac{w_k}{\|w_k\|},\quad k=1,\ldots,n,
$$

where the empty sum for $k=1$ is zero. Assuming the preceding $e_j$ are [orthonormal](../../../../orthonormal-set.md), taking the [inner product](../../../../inner-product-split.md) of $w_k$ with $e_i$, $i<k$, gives zero. Moreover $w_k\ne0$: otherwise $v_k$ would belong to the [span](../../../../linear-span.md) of $v_1,\ldots,v_{k-1}$, contrary to [linear independence](../../../../linear-independence.md). Normalization is therefore legitimate and produces an [orthonormal basis](../../../../orthonormal-basis.md). At each stage the first $k$ constructed vectors have the same [span](../../../../linear-span.md) as the first $k$ original vectors.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../split.md)
5. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
