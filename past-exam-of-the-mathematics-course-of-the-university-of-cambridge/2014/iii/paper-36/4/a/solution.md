<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $w(x)=f(x)/g(x)$ where $g(x)>0$, and set it to zero on the g-null set where $g=0$. The domination assumption makes $f=0$ there and gives $0\leq w\leq M$. Integrating it also gives $M\geq1$. For iid proposals $X_i\sim g$, the [importance sampling](../../../../../../importance-sampling.md) estimator is

$$
\boxed{\widehat\theta_1=\frac1n\sum_{i=1}^n\phi(X_i)w(X_i).}
$$

[Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) under $f$ gives $|\theta|\leq(\int\phi^2f)^{1/2}<\infty$. Direct integration proves unbiasedness, $\mathbb E_g[\phi(X)w(X)]=\theta$. Moreover

$$
\mathbb E_g[\phi(X)^2w(X)^2]=\int_{g>0}\phi(x)^2\frac{f(x)^2}{g(x)}\,dx\leq M\int\phi(x)^2f(x)\,dx<\infty.
$$

Thus

$$
\boxed{\mathbb E\widehat\theta_1=\theta,\qquad\operatorname{Var}(\widehat\theta_1)=\frac{v_{\rm IS}}n,\quad
v_{\rm IS}=\int\phi^2\frac{f^2}{g}-\theta^2.}
$$

The iid [central limit theorem](../../../../../../central-limit-theorem.md) applies to these finite-[variance](../../../../../../variance-split.md) weighted observations:

$$
\boxed{\sqrt n(\widehat\theta_1-\theta)\ \Longrightarrow\ N(0,v_{\rm IS}).}
$$

If the [variance](../../../../../../variance-split.md) is zero, this denotes the point mass at zero. This is the [bounded-weight importance-sampling moment bound](../../../../../../bounded-weight-importance-sampling-moment-bound.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
