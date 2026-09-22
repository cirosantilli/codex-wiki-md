<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The risk-free weight is $1-\mathbf1^tw$, so a zero risk-free weight requires $\mathbf1^tw=1$. Define $H=\mathbf1^t\Sigma^{-1}d$. If $H\ne0$, this condition gives $\lambda=1/H$ and

$$
\boxed{w_T=\frac{\Sigma^{-1}d}{H},\qquad
\mathbb E r_T=R+\frac A H,\qquad \operatorname{Var}(r_T)=\frac A{H^2}.}
$$

These are the requested tangent-portfolio mean and [variance](../../../../../../variance-split.md) under the usual condition $H>0$. Then $\lambda>0$, the normalized [portfolio](../../../../../../investment-portfolio.md) lies on the upper efficient ray, and its [Sharpe ratio](../../../../../../sharpe-ratio.md) is $\sqrt A$.

There is a real qualification if the data are allowed to be arbitrary. If $H=0$, the efficient risky direction has zero total risky weight, and no finite multiple makes its risky weights sum to one. If $H<0$, the formal normalized [portfolio](../../../../../../investment-portfolio.md) above has negative excess mean and lies on the lower, dominated branch; it is not an efficient tangent [portfolio](../../../../../../investment-portfolio.md) as described in the question. The [sign of the normalized tangency portfolio](../../../../../../sign-of-the-normalized-tangency-portfolio.md) must therefore be checked, rather than inferred from [positive definiteness](../../../../../../positive-definiteness.md) of $\Sigma$ alone.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
