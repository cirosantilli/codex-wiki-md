<h1 id="algebra/1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

To prove the sum is direct, suppose $\sum_{j=1}^rv_j=0$ with $v_j\in V_{\lambda_j}$. Fix $i$ and apply the polynomial in the [linear operator](../../../../../../linear-operator.md)

$$
P_i(T)=\prod_{j\neq i}(T-\lambda_jI).
$$

Every $v_j$ with $j\neq i$ is killed by one factor. On $v_i$, each factor is multiplication by $\lambda_i-\lambda_j$, giving

$$
0=P_i(T)\sum_jv_j=\left(\prod_{j\neq i}(\lambda_i-\lambda_j)\right)v_i.
$$

The scalar coefficient is nonzero because the [eigenvalues](../../../../../../eigenvalue.md) are distinct. Thus $v_i=0$ for every $i$, proving

$$
\boxed{V_{\lambda_1}+\cdots+V_{\lambda_r}=V_{\lambda_1}\oplus\cdots\oplus V_{\lambda_r}.}
$$

In particular, choosing a basis in each [eigenspace](../../../../../../eigenspace.md) yields a [linearly independent](../../../../../../linear-independence.md) combined list.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Algebra](../../../../algebra.md)
5. [2011](../../../../../2011-split.md)
6. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../../split.md)
7. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
