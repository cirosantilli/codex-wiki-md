<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Along the exact [ordinary differential equation](../../../../../../ordinary-differential-equation.md) solution, the [chain rule](../../../../../../chain-rule.md) gives $g(y)=f'(y)f(y)=y''$. Insert the exact solution into the [symmetric two-step two-derivative formula](../../../../../../symmetric-two-step-two-derivative-formula.md) and expand about the middle time $t=t_{n+1}$. Its unnormalized [local truncation error](../../../../../../local-truncation-error.md) is

$$
\begin{aligned}
\delta_h={}&y(t+h)-y(t-h)-\frac{7h}{15}[y'(t+h)+y'(t-h)]-\frac{16h}{15}y'(t)\\
&+\frac{h^2}{15}[y''(t+h)-y''(t-h)].
\end{aligned}
$$

The coefficients of $hy'$, $h^3y'''$ and $h^5y^{(5)}$ are respectively

$$
2-\frac{14}{15}-\frac{16}{15}=0,\qquad\frac13-\frac7{15}+\frac2{15}=0,\qquad\frac1{60}-\frac7{180}+\frac1{45}=0.
$$

The centered residual is an [odd function](../../../../../../odd-function.md) of $h$, so every even power cancels. The next coefficient is

$$
\frac1{2520}-\frac7{5400}+\frac1{900}=\frac1{4725},\qquad\delta_h=\frac{h^7}{4725}y^{(7)}(t)+O(h^9).
$$

Thus **the method has order six**. Its [zero-stability](../../../../../../zero-stability.md) roots at $h=0$ are the simple roots $1,-1$. With sufficiently accurate starts and smooth derivative evaluation maps, [convergence of a zero-stable multiderivative method](../../../../../../convergence-of-a-zero-stable-multiderivative-method.md) gives sixth-order error on fixed time intervals. The [first Dahlquist barrier](../../../../../../first-dahlquist-barrier.md) for ordinary [linear multistep methods](../../../../../../linear-multistep-method.md) does not apply, because this is a [multiderivative multistep method](../../../../../../multiderivative-multistep-method.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 69](../../../paper-69-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)

## ← Incoming links (1)

- [Solution](../../6/solution.md)
