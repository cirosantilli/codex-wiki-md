<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the single event

$$
\mathcal E=\bigcap_{t\geq0}\{\theta_\star\in\Theta_t\},\qquad\mathbb P(\mathcal E)\geq1-\delta.
$$

Fix a realization in $\mathcal E$. The action space is nonempty and [compact](../../../../compact-space.md), since it is a closed subset of the finite-dimensional unit ball. The [Lipschitz continuous](../../../../lipschitz-continuity.md) reward function is continuous, so there is an optimal action $x_\star\in\operatorname*{arg\,max}_{x\in\mathcal X}\mu(\langle x,\theta_\star\rangle)$. Because the same reward function is used at every time, the [pseudoregret](../../../../pseudoregret.md) is $R_n=\sum_{t=1}^n r_t$, where

$$
r_t=\mu(\langle x_\star,\theta_\star\rangle)-\mu(\langle X_t,\theta_\star\rangle)\geq0.
$$

The pair $(x_\star,\theta_\star)$ is feasible in the optimization defining $(X_t,\theta_t)$. This [optimism in the face of uncertainty](../../../../optimism-in-the-face-of-uncertainty.md) gives

$$
\mu(\langle x_\star,\theta_\star\rangle)\leq\mu(\langle X_t,\theta_t\rangle),
\qquad
r_t\leq L|\langle X_t,\theta_t-\theta_\star\rangle|.
$$

For any [positive-definite matrix](../../../../positive-definite-matrix.md) $V$, the ordinary [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) applied to $V^{-1/2}x$ and $V^{1/2}z$ proves

$$
|\langle x,z\rangle|\leq|x|_{V^{-1}}|z|_V.
$$

Both $\theta_t$ and $\theta_\star$ belong to the same [confidence ellipsoid](../../../../confidence-ellipsoid.md) $\Theta_{t-1}$. The [triangle inequality](../../../../triangle-inequality.md) for the [norm](../../../../norm.md) associated with this [weighted Euclidean inner product](../../../../weighted-euclidean-inner-product.md) therefore gives

$$
|\theta_t-\theta_\star|_{V_{t-1}}
\leq|\theta_t-\widehat\theta_{t-1}|_{V_{t-1}}
+|\widehat\theta_{t-1}-\theta_\star|_{V_{t-1}}
\leq2\beta_{t-1}(\delta),
$$

and hence $r_t\leq2L\beta_{t-1}(\delta)|X_t|_{V_{t-1}^{-1}}$. Monotonicity of $\beta_t(\delta)$ and another [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) now yield

$$
\begin{aligned}
R_n&\leq2L\beta_n(\delta)\sum_{t=1}^n|X_t|_{V_{t-1}^{-1}}\\
&\leq\boxed{2L\beta_n(\delta)\sqrt{n\sum_{t=1}^n|X_t|_{V_{t-1}^{-1}}^2}}.
\end{aligned}
$$

This reasoning holds on $\mathcal E$ for every $n$ simultaneously, proving the asserted probability. In combination with part (a), it also gives

$$
R_n\leq2L\beta_n(\delta)\sqrt{2nd\log\left(1+\frac n{d\lambda}\right)}.
$$

Only the supplied simultaneous [confidence set](../../../../confidence-region.md) coverage and the optimistic choice are needed here. No claim that the displayed linear estimator is automatically a suitable estimator for a nonlinear link is required: its coverage was an explicit hypothesis.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the algorithmic foundations of learning course of the University of Oxford](../../../split.md)
5. [Algorithmic foundations of learning course of the University of Oxford](../../../../algorithmic-foundations-of-learning-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
