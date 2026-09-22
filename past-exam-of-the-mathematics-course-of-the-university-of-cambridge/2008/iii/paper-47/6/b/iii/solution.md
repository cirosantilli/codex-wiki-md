<h1 id="6/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Initialize $0<\theta^{(0)}<1$. At each iteration first compute $y_3^{(t)}=x_3\theta^{(t)}/(2+\theta^{(t)})$ by the conditional [expectation](../../../../../../../expected-value.md) above. The M-step applies the complete-data [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md) to the filled counts, giving

$$
\boxed{\theta^{(t+1)}=
\frac{x_2+x_3\theta^{(t)}/(2+\theta^{(t)})}
{x_1+x_2+x_3\theta^{(t)}/(2+\theta^{(t)})}.}
$$

Repeat until convergence. If all counts are zero, the [likelihood function](../../../../../../../likelihood-function.md) is constant and any parameter can be retained. For a nonempty sample an interior start makes the displayed denominator positive.

Here the three observed cell probabilities are $(1-\theta)/2$, $\theta/4$ and $(2+\theta)/4$, so the observed [log-likelihood](../../../../../../../log-likelihood.md) is

$$
\ell(\theta)=x_1\log(1-\theta)+x_2\log\theta+x_3\log(2+\theta)+C.
$$

For a nonempty sample its second derivative on $(0,1)$ is

$$
\ell''(\theta)=-\frac{x_1}{(1-\theta)^2}-\frac{x_2}{\theta^2}-\frac{x_3}{(2+\theta)^2}<0.
$$

Thus the [maximum-likelihood estimator](../../../../../../../maximum-likelihood-estimator.md) is unique, allowing a boundary maximum. To verify that the iteration actually finds it, let $u(\theta)=x_3\theta/(2+\theta)$ and $F(\theta)=(x_2+u(\theta))/(x_1+x_2+u(\theta))$. Then $F'(\theta)=x_1u'(\theta)/(x_1+x_2+u(\theta))^2\geq0$, and

$$
F(\theta)-\theta=\frac{\theta(1-\theta)\ell'(\theta)}{x_1+x_2+u(\theta)}.
$$

If the maximum is interior, this identity moves each iterate towards it, and monotonicity of $F$ prevents crossing it. The bounded monotone iterates converge; continuity makes their limit a fixed point, and strict concavity makes that fixed point the maximum. If the maximum is at zero or one, the sign of $\ell'$ gives the same monotone convergence towards the appropriate endpoint. In the special case $x_1=0$, $F$ is identically one whenever its denominator is positive, so the maximum is reached in one step. An interior initialization avoids the possible spurious zero fixed point when $x_2=0$; starting at zero can otherwise trap the iteration even when the true maximum is positive.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Paper 47](../../../../paper-47-split.md)
5. [Iii](../../../../split.md)
6. [2008](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
