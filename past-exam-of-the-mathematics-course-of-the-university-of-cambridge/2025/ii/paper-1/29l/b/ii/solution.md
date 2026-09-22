<h1 id="29l/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Since $\mathbb EX_i=1/\theta$ and $\operatorname{Var}(X_i)=1/\theta^2$, the central [limit](../../../../../../../limit-of-a-function.md) theorem gives

$$
\sqrt n(\overline X-1/\theta)\Rightarrow N(0,1/\theta^2).
$$

Applying the [delta method](../../../../../../../delta-method.md) to $g(x)=1/x$ yields

$$
\sqrt n(\widehat\theta_n-\theta)\Rightarrow N(0,\theta^2).
$$

Thus, with $z_{1-\alpha/2}=\Phi^{-1}(1-\alpha/2)$, an asymptotic interval centered at the MLE is

$$
C_n=\left[\widehat\theta_n-z_{1-\alpha/2}\frac{\widehat\theta_n}{\sqrt n},
\widehat\theta_n+z_{1-\alpha/2}\frac{\widehat\theta_n}{\sqrt n}\right],
$$

optionally intersected with $(0,\infty)$. Slutsky's theorem gives coverage tending to $1-\alpha$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [29L](../../../29l.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2025](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
