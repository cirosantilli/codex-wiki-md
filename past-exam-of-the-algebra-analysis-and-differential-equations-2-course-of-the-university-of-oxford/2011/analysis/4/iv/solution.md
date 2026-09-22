<h1 id="analysis/4/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

For each triangle compactly contained in $U$, part (i) permits the interchange of the series and its boundary integral. [Cauchy's integral theorem](../../../../../cauchy-s-integral-theorem.md) makes every term zero. The uniform limit is continuous, so [Morera's theorem](../../../../../morera-s-theorem.md) yields that $f$ is holomorphic on $U$.

For the final application, each function $(z-k)^{-2}$ is holomorphic away from its pole. Fix a positive integer $n$. For $z\in U_n$ and $k>2n$,

$$
|z-k|\geq k-|z|>k-n\geq k/2,\qquad
\left|\frac1{(z-k)^2}\right|\leq\frac4{k^2}.
$$

The numerical series $\sum_{k>2n}4/k^2$ converges, so the [Weierstrass M-test](../../../../../weierstrass-m-test.md) gives [uniform convergence](../../../../../uniform-convergence.md) of the tail on $U_n$. Adding the finitely many initial terms preserves [uniform convergence](../../../../../uniform-convergence.md). Those initial terms need not be bounded near their excluded poles; only the tail needs the uniform bound. By the first conclusion, the full sum is holomorphic on each $U_n$. Their union is $\mathbb C\setminus\mathbb N$, hence

$$
\boxed{\sum_{k=1}^\infty\frac1{(z-k)^2}\text{ is holomorphic on }\mathbb C\setminus\mathbb N.}
$$

## ↑ Ancestors (13)

1. [Iv](../iv.md)
2. [4](../../4.md)
3. [Analysis](../../../analysis.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
