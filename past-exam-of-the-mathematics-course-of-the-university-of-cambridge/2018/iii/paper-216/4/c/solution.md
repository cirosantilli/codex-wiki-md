<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Fix the observed $Y$, let $L(\theta)=p_\theta(Y)$, and let $q_0(z)=p_{\theta_0}(z\mid Y)$. The E-step forms

$$
Q(\theta\mid\theta_0)=\int q_0(z)\log p_\theta(Y,z)\,dz.
$$

For finite expected log-likelihoods and $L(\theta_0)>0$, the [Jensen inequality](../../../../../../jensen-s-inequality.md) gives

$$
\begin{aligned}
\log\frac{L(\theta)}{L(\theta_0)}
&\geq\log\int q_0(z)\frac{p_\theta(Y,z)}{p_{\theta_0}(Y,z)}\,dz\\
&\geq\int q_0(z)\log\frac{p_\theta(Y,z)}{p_{\theta_0}(Y,z)}\,dz\\
&=Q(\theta\mid\theta_0)-Q(\theta_0\mid\theta_0).
\end{aligned}
$$

The first inequality allows additional mass outside the old complete-data support; it is equality when the relevant supports coincide. Ratios are taken on the support of $q_0$. If a candidate assigns zero density on positive $q_0$-mass, its $Q$ is minus infinity and it cannot be an improving finite M-step.

An M-step of the [expectation-maximization algorithm](../../../../../../expectation-maximization-algorithm.md) chooses $\theta_1$ with $Q(\theta_1\mid\theta_0)\geq Q(\theta_0\mid\theta_0)$, so

$$
\boxed{\log L(\theta_1)\geq\log L(\theta_0),\qquad L(\theta_1)\geq L(\theta_0).}
$$

This [EM likelihood monotonicity](../../../../../../em-likelihood-monotonicity.md) also holds for a generalized M-step that merely increases $Q$, rather than maximizing it exactly. It is a statement about the observed-data [likelihood function](../../../../../../likelihood-function.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 216](../../../paper-216-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
