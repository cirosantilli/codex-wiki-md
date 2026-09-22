<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a positive Hermitian matrix,

$$
\boxed{\kappa(A)=\frac{\lambda_{\max}}{\lambda_{\min}}}.
$$

The [HHL algorithm](../../../../../../hhl-algorithm.md) phase-estimates $A$, performs a controlled rotation with amplitude proportional to $1/\lambda_i$, uncomputes the estimate, and postselects the rotation ancilla. Resolving the smallest eigenvalue requires phase-estimation precision $O(\lambda_{\min})$ and evolution time $\Omega(1/\lambda_{\min})$. Since $\lambda_{\max}\leq1$, this contributes a dependence at least linear in $\kappa$.

The controlled rotation must use a scale $C\leq\lambda_{\min}$. In the worst input direction its success probability is of order

$$
\frac{C^2}{\lambda_{\max}^2}=O(\kappa^{-2}),
$$

so obtaining constant success by [amplitude amplification](../../../../../../amplitude-amplification.md) costs another $O(\kappa)$ factor. Thus a runtime polynomial in $\log N$ requires

$$
\boxed{\kappa=O(\operatorname{poly}(\log N))}.
$$

An exponentially ill-conditioned matrix would require exponentially fine phase resolution or exponentially many amplification steps.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 324](../../../paper-324-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
