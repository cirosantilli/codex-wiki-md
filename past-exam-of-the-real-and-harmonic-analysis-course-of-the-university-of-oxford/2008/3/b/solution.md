<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Set $C=\sup_k\|\mu_k\|$. Given $f\in C(\mathbb T)$, choose $g\in X$ with $\|f-g\|_\infty<\varepsilon$. Then

$$
\left|\int f\,d\mu_k-\int f\,d\mu\right|\leq(C+\|\mu\|)\varepsilon+\left|\int g\,d\mu_k-\int g\,d\mu\right|.
$$

Take the upper limit in $k$ and then $\varepsilon\downarrow0$. Thus **convergence on the dense test family suffices**; no assumption that $X$ is a vector space is needed.

For nonempty compact $K$, put $f_j(x)=\max\{0,1-j\operatorname{dist}(x,K)\}$. These [continuous functions](../../../../continuous-function.md) decrease to $\mathbf1_K$ and satisfy $\mu_k(K)\leq\int f_j\,d\mu_k$. Consequently $\limsup_k\mu_k(K)\leq\int f_j\,d\mu$ for every $j$. [Dominated convergence](../../../../dominated-convergence-theorem.md) for the finite [positive measure](../../../../positive-measure.md) $\mu$ yields

$$
\boxed{\limsup_k\mu_k(K)\leq\mu(K).}
$$

The empty-set case is immediate. Positivity is essential for the comparison with these cutoff functions.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the real and harmonic analysis course of the University of Oxford](../../../split.md)
5. [Real and harmonic analysis course of the University of Oxford](../../../../real-and-harmonic-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
