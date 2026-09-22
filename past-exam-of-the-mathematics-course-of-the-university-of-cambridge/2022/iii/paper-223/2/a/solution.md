<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The normal location score is $x-\theta$. Under a bound on [gross-error sensitivity](../../../../../../gross-error-sensitivity.md), the variance-minimizing influence curve clips this score. For $b>0$, define the [Huber score](../../../../../../huber-score.md)

$$
\psi_b(u)=[u]_{-b}^{b}
=\max(-b,\min(u,b)).
$$

The optimal [B-robust estimator](../../../../../../b-robust-estimator.md) is the [Huber location estimator](../../../../../../huber-location-estimator.md) $\widehat\theta_b$ defined by

$$
\sum_{i=1}^n\psi_b(x_i-\widehat\theta_b)=0.
$$

Equivalently, it has the explicit optimization form

$$
\widehat\theta_b
=\underset{t\in\mathbb R}{\arg\min}
\sum_{i=1}^n\rho_b(x_i-t),
$$

where the [Huber loss](../../../../../../huber-loss.md) is

$$
\rho_b(u)=
\begin{cases}
u^2/2,&|u|\leq b,\\
b|u|-b^2/2,&|u|>b.
\end{cases}
$$

At $N(\theta,1)$ its normalized influence function is

$$
\boxed{\operatorname{IF}(x;T_b,F_\theta)
=\frac{\psi_b(x-\theta)}{\mathbb P(|Z|\leq b)},
\qquad Z\sim N(0,1).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
