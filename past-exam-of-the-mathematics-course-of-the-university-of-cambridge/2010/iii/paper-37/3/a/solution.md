<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Bernoulli distribution](../../../../../../bernoulli-distribution.md) probability mass function is

$$
\Pr(Y_i=y_i)=p_i^{y_i}(1-p_i)^{1-y_i}=\exp\left\{y_i\log\frac{p_i}{1-p_i}+\log(1-p_i)\right\}.
$$

Writing $\theta_i=\log[p_i/(1-p_i)]$ gives $p_i=e^{\theta_i}/(1+e^{\theta_i})$ and $\log(1-p_i)=-\log(1+e^{\theta_i})$. Therefore the [exponential family](../../../../../../exponential-family-split.md) representation has

$$
\boxed{\theta_i=\operatorname{logit}(p_i)=\beta^Tx_i,\quad b(\theta)=\log(1+e^\theta),\quad\phi=1,\quad c(y,\phi)=0.}
$$

The [logit link](../../../../../../logit.md) is the canonical link.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
