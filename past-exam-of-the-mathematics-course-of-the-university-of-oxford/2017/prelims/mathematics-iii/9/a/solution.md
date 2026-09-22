<h1 id="9/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the corrected decomposition

$$
y_{ij}-w_j=(y_{ij}-\mu_j)+(\mu_j-w_j).
$$

The hint's minus sign before $(\mu_j-w_j)$ is a typographical error. Squaring, summing, and using $\sum_i(y_{ij}-\mu_j)=0$ for each coordinate gives the [centroid sum-of-squares identity](../../../../../../centroid-sum-of-squares-identity.md)

$$
\sum_{i,j}(y_{ij}-w_j)^2
=\sum_{i,j}(y_{ij}-\mu_j)^2
+2\sum_j(\mu_j-w_j)\underbrace{\sum_i(y_{ij}-\mu_j)}_{0}
+m\sum_j(\mu_j-w_j)^2.
$$

Since $m>0$ and $w\ne\mu$, the final term is strictly positive. Hence

$$
\boxed{\sum_{i,j}(y_{ij}-\mu_j)^2<\sum_{i,j}(y_{ij}-w_j)^2.}
$$

Thus the [centroid](../../../../../../centroid.md) uniquely minimizes the sum of squared [Euclidean distances](../../../../../../euclidean-distance.md) to the observations.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [9](../../9.md)
3. [Mathematics III](../../../mathematics-iii-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
