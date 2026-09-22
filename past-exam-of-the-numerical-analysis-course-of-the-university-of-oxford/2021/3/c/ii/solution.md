<h1 id="3/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

As appropriate for a genuine $k$-step [linear multistep method](../../../../../linear-multistep-method-split.md), take $\alpha_k\ne0$. Suppose the [characteristic polynomial](../../../../../characteristic-polynomial.md) has a [polynomial root](../../../../../root-of-a-polynomial.md) $\xi$ with [modulus](../../../../../modulus.md) $|\xi|>1$. From $\rho(\xi)=0$ and the [triangle inequality](../../../../../triangle-inequality.md),

$$
\begin{aligned}
|\alpha_k||\xi|^k
&=\left|\sum_{j=0}^{k-1}\alpha_j\xi^j\right|\\
&\leq\sum_{j=0}^{k-1}|\alpha_j||\xi|^j\\
&\leq|\xi|^{k-1}\sum_{j=0}^{k-1}|\alpha_j|\\
&\leq|\alpha_k||\xi|^{k-1}.
\end{aligned}
$$

Dividing by the positive number $|\alpha_k||\xi|^{k-1}$ gives $|\xi|\leq1$, a contradiction. Hence

$$
\boxed{|\xi_i|\leq1\qquad(i=1,\ldots,k).}
$$

The nonzero leading [coefficient](../../../../../coefficient.md) matters: if $\alpha_k=0$, the assumed inequality forces all the $\alpha_j$ to vanish, so $\rho$ is the zero [polynomial](../../../../../polynomial-split.md) rather than a [characteristic polynomial](../../../../../characteristic-polynomial.md) with $k$ roots. This degenerate case does not define the method in the question.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the numerical analysis course of the University of Oxford](../../../../split.md)
6. [Numerical analysis course of the University of Oxford](../../../../../numerical-analysis-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
