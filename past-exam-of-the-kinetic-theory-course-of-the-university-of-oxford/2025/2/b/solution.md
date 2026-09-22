<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A_0=f_0(0)$, $\delta=v_2-v_1$, $V=v_0+\delta$ and $K=k^2\lambda_{\mathrm{De}}^2$. Use the [Debye length](../../../../debye-length.md) convention of the paper, $\lambda_{\mathrm{De}}=v_0/\omega_{\mathrm{pe}}$. On the candidate intervals in [a](../a.md), the [Landau contour](../../../../landau-contour.md) contributes no imaginary part. The piecewise constant slopes give

$$
\begin{aligned}
I(u)&=\int\frac{f_0'(v)}{v-u}\,dv\\
&=\frac{A_0}{v_0}\left[\int_{-v_0}^{0}\frac{dv}{v-u}-\int_0^{v_1}\frac{dv}{v-u}-\int_{v_2}^{V}\frac{dv}{v-u}\right]\\
&=\frac{A_0}{v_0}\left[2\ln|u|-\ln|v_0+u|-\ln|v_1-u|-\ln|V-u|+\ln|v_2-u|\right].
\end{aligned}
$$

Since $n_0=v_0A_0$, setting the [dielectric function](../../../../dielectric-function.md) to zero yields

$$
\boxed{\ln\frac{u^2|v_2-u|}{|v_0+u|\,|v_1-u|\,|V-u|}=K.}
$$

The absolute values express the real response on the allowed intervals. Solving this real equation inside a sloping portion of $f_0$ would not satisfy the imaginary part of the [dielectric function](../../../../dielectric-function.md).

An exact algebraic form will also make the number of undamped branches clear. Define

$$
A=v_0^2+\delta(v_0-v_1),\qquad B=v_0v_1V,\qquad q=1-e^{-K}.
$$

On each allowed interval, the quantity inside the logarithm equals $u^2(u-v_2)/[(u+v_0)(u-v_1)(u-V)]$. Exponentiating and using

$$
(u+v_0)(u-v_1)(u-V)=u^2(u-v_2)-Au+B
$$

gives the [cubic equation](../../../../cubic-equation.md)

$$
q\,u^2(u-v_2)-Au+B=0.
$$

For every $k>0$, the logarithm runs from $0$ to $+\infty$ on $(-\infty,-v_0)$, from $+\infty$ to $-\infty$ on $(v_1,v_2)$, and from $+\infty$ to $0$ on $(V,\infty)$. The [intermediate value theorem](../../../../intermediate-value-theorem.md) supplies a root in each interval, and the [cubic equation](../../../../cubic-equation.md) permits at most three. Thus there is exactly one undamped branch in each interval.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the kinetic theory course of the University of Oxford](../../../split.md)
5. [Kinetic theory course of the University of Oxford](../../../../kinetic-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
