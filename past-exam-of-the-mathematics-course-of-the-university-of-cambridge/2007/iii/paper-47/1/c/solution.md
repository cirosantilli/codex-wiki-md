<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At equal spacing $h$, the adjacent increments of an affine mean profile are all $\beta h$. Their differences are therefore zero. Define the $(p-2)\times p$ matrix $B$ whose row associated with the interior time $i$ has coefficients $1,-2,1$ in columns $i-1,i,i+1$. Then

$$
(B\mu)_{i-1}=\mu_{i-1}-2\mu_i+\mu_{i+1}=0.
$$

Conversely these equations make all adjacent first differences equal, so $\mu_i$ is affine in $i$, equivalently affine in the equally spaced times. Thus the restriction is exactly $B\mu=0$, not just a necessary condition. Its [null space](../../../../../../kernel-of-a-linear-map.md) has basis $\mathbf1$ and $t=(t_1,\ldots,t_p)^T$, so $B$ has [rank](../../../../../../rank-one-quadratic-form.md) $r=p-2$.

For $p\ge3$ and $n>r$, the [second-difference test of a linear mean profile](../../../../../../second-difference-test-of-a-linear-mean-profile.md) is the [Hotelling test of linear hypotheses](../../../../../../hotelling-test-of-linear-hypotheses.md) with

$$
\boxed{T_B^2=n(B\bar X)^T(BSB^T)^{-1}(B\bar X),\qquad
\frac{n-r}{r(n-1)}T_B^2\sim F_{r,n-r}.}
$$

Reject the affine-profile hypothesis when the scaled statistic exceeds its level-$\eta$ upper [F-distribution](../../../../../../f-distribution.md) critical value. This removes the nuisance intercept and slope without estimating them separately.

For unequal ordered distinct times, put $h_i=t_{i+1}-t_i>0$ and replace each second-difference row by the adjacent-slope contrast

$$
\frac{\mu_{i+1}-\mu_i}{h_i}-\frac{\mu_i-\mu_{i-1}}{h_{i-1}}.
$$

Its three coefficients are $1/h_{i-1}$, $-(1/h_{i-1}+1/h_i)$ and $1/h_i$. Vanishing means all adjacent slopes agree, again giving [null space](../../../../../../kernel-of-a-linear-map.md) $\operatorname{span}(\mathbf1,t)$ and [rank](../../../../../../rank-one-quadratic-form.md) $p-2$. Use this new $B$ in the same statistic and null distribution. For $p\le2$, every mean profile at distinct times is affine, so there is no lack-of-linearity restriction to test.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
