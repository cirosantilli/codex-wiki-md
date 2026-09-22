<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For fixed $\varepsilon>0$, let the [quantum typical subspace](../../../../../../quantum-typical-subspace.md) $\mathcal T_\varepsilon^{(n)}$ be spanned by the product eigenvectors with nonzero eigenvalues satisfying

$$
2^{-n(S(\pi)+\varepsilon)}\leq\lambda_{\mathbf j}\leq2^{-n(S(\pi)-\varepsilon)}.
$$

Equivalently their spectral information $-n^{-1}\log_2\lambda_{\mathbf j}$ lies within $\varepsilon$ of $S(\pi)$. Denote its [orthogonal projection](../../../../../../orthogonal-projection.md) by $P_\varepsilon^{(n)}$.

The [typical subspace theorem](../../../../../../typical-subspace-theorem.md) states that for every $\delta>0$ there is $n_0$ such that for $n\geq n_0$,

$$
\boxed{\operatorname{Tr}(\pi^{\otimes n}P_\varepsilon^{(n)})\geq1-\delta,\qquad
(1-\delta)2^{n(S(\pi)-\varepsilon)}\leq\dim\mathcal T_\varepsilon^{(n)}\leq2^{n(S(\pi)+\varepsilon)}.}
$$

Also the operator bounds on its range are

$$
2^{-n(S(\pi)+\varepsilon)}P_\varepsilon^{(n)}\leq P_\varepsilon^{(n)}\pi^{\otimes n}P_\varepsilon^{(n)}\leq2^{-n(S(\pi)-\varepsilon)}P_\varepsilon^{(n)}.
$$

To see the concentration statement, sample $j_s$ independently with probabilities $\lambda_j$. The mean of $-\log_2\lambda_{j_s}$ is $S(\pi)$, so the [weak law of large numbers](../../../../../../weak-law-of-large-numbers.md) gives typical probability tending to one. Zero-eigenvalue letters have probability zero and are excluded. The dimension bounds follow by summing the upper and lower typical eigenvalue bounds and using the typical mass between $1-\delta$ and $1$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 34](../../../paper-34-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
