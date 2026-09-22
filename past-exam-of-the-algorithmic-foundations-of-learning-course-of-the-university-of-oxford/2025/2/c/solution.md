<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\mathcal G_t=\sigma(X_1,\ldots,X_t)$. Under $P_{\theta_\star}$, the true [probability density function](../../../../probability-density-function.md) is positive and finite at every observation almost surely. Define the sequential [likelihood ratio](../../../../likelihood-ratio.md)

$$
M_0=1,\qquad
M_t=\prod_{s=1}^t\frac{p_{\widehat\theta_{s-1}}(X_s)}{p_{\theta_\star}(X_s)}.
$$

A zero numerator sets the product to zero thereafter. Thus $M_t$ is a well-defined nonnegative process, and $L_t(\theta_\star)=\log M_t$, with $\log0=-\infty$.

The next observation is [independent](../../../../independent-random-variables.md) of $\mathcal G_{s-1}$, while $\widehat\theta_{s-1}$ is [measurable](../../../../measurability.md) with respect to that [sigma-algebra](../../../../sigma-algebra.md). Its [conditional expectation](../../../../conditional-expectation.md) is therefore

$$
\begin{aligned}
\mathbb E_{\theta_\star}\left[\left.
\frac{p_{\widehat\theta_{s-1}}(X_s)}{p_{\theta_\star}(X_s)}\right|\mathcal G_{s-1}\right]
&=\int_{\{p_{\theta_\star}>0\}}
p_{\widehat\theta_{s-1}}(x)\,d\mu(x)\\
&\leq1.
\end{aligned}
$$

Consequently $\mathbb E(M_s\mid\mathcal G_{s-1})\leq M_{s-1}$; induction also gives $\mathbb EM_s\leq1$. Thus $(M_t)$ is a nonnegative [supermartingale](../../../../supermartingale.md) for the [filtration](../../../../filtration-probability-theory.md) $(\mathcal G_t)$. It need not be a [martingale](../../../../martingale-split.md): an alternative distribution can put mass outside the support of the true distribution.

The [maximal inequality for a nonnegative supermartingale](../../../../maximal-inequality-for-a-nonnegative-supermartingale.md), the corresponding form of the [Ville inequality](../../../../ville-inequality.md), gives

$$
\begin{aligned}
\mathbb P_{\theta_\star}\{\exists t\geq0:\theta_\star\notin\Theta_t\}
&=\mathbb P_{\theta_\star}\{\exists t\geq0:L_t(\theta_\star)\geq\log(1/\delta)\}\\
&\leq\mathbb P_{\theta_\star}\{\sup_{t\geq0}M_t\geq1/\delta\}\\
&\leq\boxed{\delta\mathbb EM_0=\delta}.
\end{aligned}
$$

The strict inequality in the definition of the [confidence set](../../../../confidence-region.md) correctly becomes a non-strict crossing event.

There is a minor definitional omission in the source: for false candidates $\theta$, the printed sum of [log-likelihood ratios](../../../../log-likelihood-ratio.md) can involve $0/0$ or both infinite signs. To define the entire [confidence set](../../../../confidence-region.md) without a positivity assumption, use the logarithm of the ratio of the two full products, $\prod_s p_{\widehat\theta_{s-1}}(X_s)$ and $\prod_s p_\theta(X_s)$, taking $0/a=0$ for $a>0$, $a/0=+\infty$ for $a>0$, and, for example, $0/0=1$. This is a measurable extension of the printed formula wherever that formula is defined. The choice at $0/0$ cannot affect coverage of the truth, since its full denominator is positive almost surely. Alternatively, strict positivity of every density on the common support removes the omission.

## ↑ Ancestors (12)

1. [C](../c.md)
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
