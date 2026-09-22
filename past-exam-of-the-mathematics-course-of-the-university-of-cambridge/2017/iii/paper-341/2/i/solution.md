<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Insert an exact smooth [solution of a differential equation](../../../../../../solution-of-a-differential-equation.md) and expand about $t=t_{n+2}$. The unscaled [local truncation error](../../../../../../local-truncation-error.md), with every term moved to the left, is

$$
d_h(t)=\frac{1-7\alpha}{6}h^3y^{(3)}(t)
+\frac{15\alpha-1}{24}h^4y^{(4)}(t)+O(h^5).
$$

Here the constant, first-[derivative](../../../../../../derivative.md), and second-[derivative](../../../../../../derivative.md) terms all cancel, using the [chain rule](../../../../../../chain-rule.md) identity $y''=f'(y)f(y)$. Hence the formal defect convention $d_h=O(h^{p+1})$ gives

$$
\boxed{p=3\quad(\alpha=1/7),\qquad p=2\quad(\alpha\ne1/7)}.
$$

At $\alpha=1/7$, the coefficient of $h^4y^{(4)}$ is $1/21$, so there is no further cancellation. At any other $\alpha$, the cubic coefficient is nonzero.

There is a degeneracy at $\alpha=1$: both the first-[derivative](../../../../../../derivative.md) coefficient and $\rho'(1)$ vanish. The raw defect still has the displayed formal order two, but it cannot be normalized by $(1-\alpha)h$ into an ordinary first-order [consistency of a numerical method](../../../../../../consistency-of-a-numerical-method.md) test. Thus a convention requiring this nondegenerate normalization would leave the ODE order undefined at $\alpha=1$. In either convention, it is not a convergent approximation to arbitrary initial-value data; the next part explains why.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 341](../../../paper-341-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
