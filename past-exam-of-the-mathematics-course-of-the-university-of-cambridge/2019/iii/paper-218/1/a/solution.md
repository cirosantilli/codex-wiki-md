<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $H_i$ be the number healthy among $m_i=25$ patients and $Y_i=H_i/m_i$. The fitted [grouped-binomial logistic regression](../../../../../../grouped-binomial-logistic-regression.md) is

$$
H_i\sim\operatorname{Binomial}(m_i,p_i),
\qquad
\operatorname{logit}(p_i)=\beta_0+\beta_S\mathbf1_{\{\mathrm{sex}=M\}}+\beta_T\mathbf1_{\{\mathrm{treatment}=1\}}.
$$

For $y=h/m$ its mass has [exponential dispersion family](../../../../../../exponential-dispersion-model.md) form

$$
\Pr(Y=y)=\exp\left\{
\frac{y\theta-b(\theta)}{\phi}+c(y,\phi)
\right\},
$$

where

$$
\theta=\log\frac p{1-p},\qquad b(\theta)=\log(1+e^\theta),
\qquad\phi=\frac1m.
$$

Thus $\mathbb EY=p=b'(\theta)$ and

$$
\operatorname{Var}(Y)=\phi V(p),
\qquad\boxed{V(p)=p(1-p).}
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 218](../../../paper-218-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
