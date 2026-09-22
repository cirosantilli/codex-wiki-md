<h1 id="22f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each $k$, choose $n_k$ with $\lambda(A\setminus E_{n_k}^{(k)})\le\varepsilon2^{-k-1}$ and set $B=\bigcap_{k\ge1}E_{n_k}^{(k)}$. [Countable subadditivity](../../../../../../countable-subadditivity-of-a-measure.md) gives $\lambda(A\setminus B)\le\varepsilon/2$. For any tolerance $\delta>0$, choose $k$ with $1/k<\delta$. For all $m\ge n_k$ and every $x\in B$, $|f_m(x)-f(x)|\le1/k$, proving [uniform convergence](../../../../../../uniform-convergence.md) on $B$.

If the [functions](../../../../../../function-split.md) are Borel measurable, $B$ itself is Borel and we can take $A_\varepsilon=B$. If “measurable” is interpreted in the completed Lebesgue sense, use [regularity of Lebesgue measure](../../../../../../regularity-of-lebesgue-measure.md) to choose a Borel subset $A_\varepsilon\subseteq B$ differing from $B$ by a null [set](../../../../../../set-split.md); the same measure bound and [uniform convergence](../../../../../../uniform-convergence.md) hold. Thus the requested Borel conclusion is valid under either convention. This proves the finite-measure [Egorov theorem](../../../../../../egorov-s-theorem.md).

For an infinite-measure counterexample take $A=[0,\infty)$ and $f_n=\mathbf1_{[n,\infty)}$. It converges pointwise to zero. Any subset of $A$ with complement of finite measure intersects every infinite tail $[n,\infty)$, so the supremum of $f_n$ there is one for every $n$. Hence **finite measure is essential to the conclusion**.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [22F](../../22f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
