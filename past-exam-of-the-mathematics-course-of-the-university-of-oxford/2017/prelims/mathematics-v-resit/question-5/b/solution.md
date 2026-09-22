<h1 id="question-5/b/solution">Solution</h1>

↑ **Parent:** [b](../b.md)

**The printed arguments $x-t$ and $x+t$ assume unit wave speed.** For the stated [wave equation](../../../../../../wave-equation-split.md) with general $c>0$, the correct arguments are $x-ct$ and $x+ct$, as in the paper's subsequent formula. Equivalently, use rescaled time $\widetilde t=ct$ to obtain the printed unit-speed form.

Introduce coordinates $\xi=x-ct$, $\eta=x+ct$ along the [characteristic lines for the one-dimensional wave equation](../../../../../../characteristic-line-for-the-one-dimensional-wave-equation.md), and write $u(x,t)=U(\xi,\eta)$. The [chain rule](../../../../../../chain-rule.md) gives

$$
\partial_x=\partial_\xi+\partial_\eta,\qquad
\partial_t=-c\partial_\xi+c\partial_\eta,
$$

so the [wave equation](../../../../../../wave-equation-split.md) becomes

$$
u_{tt}-c^2u_{xx}=-4c^2U_{\xi\eta}=0.
$$

Thus $U_\xi$ is independent of $\eta$, and [integration](../../../../../../integral-split.md) gives the [countertravelling decomposition of the one-dimensional wave equation](../../../../../../countertravelling-decomposition-of-the-one-dimensional-wave-equation.md)

$$
\boxed{u(x,t)=F(x-ct)+G(x+ct)}.
$$

Conversely, differentiating this expression twice verifies the [wave equation](../../../../../../wave-equation-split.md) for any sufficiently differentiable $F,G$.

The two [initial conditions](../../../../../../initial-condition.md) give

$$
F(x)+G(x)=f(x),\qquad -cF'(x)+cG'(x)=g(x).
$$

Differentiating the first and solving these two equations for the [derivatives](../../../../../../derivative.md) gives

$$
F'(x)=\frac12f'(x)-\frac1{2c}g(x),\qquad
G'(x)=\frac12f'(x)+\frac1{2c}g(x).
$$

For a fixed reference point $x_0$, their [antiderivatives](../../../../../../antiderivative.md) can be written

$$
F(s)=\frac12f(s)-\frac1{2c}\int_{x_0}^s g(q)\,dq+C,\qquad
G(s)=\frac12f(s)+\frac1{2c}\int_{x_0}^s g(q)\,dq-C.
$$

Substituting the two travelling arguments cancels the constants and combines the [integrals](../../../../../../integral-split.md). This proves [D'Alembert's formula](../../../../../../d-alembert-s-formula.md) with initial velocity:

$$
\boxed{u(x,t)=\frac12\bigl[f(x-ct)+f(x+ct)\bigr]
+\frac1{2c}\int_{x-ct}^{x+ct}g(s)\,ds}.
$$

At $t=0$ the [integral](../../../../../../integral-split.md) vanishes, giving $u=f$; differentiating by the [fundamental theorem of calculus](../../../../../../fundamental-theorem-of-calculus.md) gives $u_t=g$ there. These checks also fix the sign and the factor $1/(2c)$.

## ↑ Ancestors (12)

1. [b](../b.md)
2. [Question 5](../../question-5.md)
3. [Mathematics V resit](../../../mathematics-v-resit-split.md)
4. [Prelims](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Oxford](../../../../../split.md)
7. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
