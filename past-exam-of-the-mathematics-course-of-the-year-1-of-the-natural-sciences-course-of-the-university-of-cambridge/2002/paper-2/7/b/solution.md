<h1 id="7/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $y(\theta)=Y(x)$ with $x=\cos\theta$. By the [chain rule](../../../../../chain-rule.md),

$$
\frac{dy}{d\theta}=-\sin\theta\,Y_x,\qquad\frac{d^2y}{d\theta^2}=-\cos\theta\,Y_x+\sin^2\theta\,Y_{xx}.
$$

The terms involving $Y_x$ cancel in the original [ordinary differential equation](../../../../../ordinary-differential-equation.md), leaving

$$
\sin\theta\,y_{\theta\theta}-\cos\theta\,y_\theta+2y\sin^3\theta=\sin^3\theta\,(Y_{xx}+2Y)=0.
$$

On each interval where $\sin\theta\ne0$, the transformed [linear ordinary differential equation](../../../../../linear-ordinary-differential-equation-split.md) is $Y_{xx}+2Y=0$. Its [characteristic equation](../../../../../characteristic-equation-of-a-constant-coefficient-differential-equation.md) has roots $\pm i\sqrt2$, yielding

$$
\boxed{y(\theta)=C_1\cos(\sqrt2\cos\theta)+C_2\sin(\sqrt2\cos\theta).}
$$

Direct substitution shows these expressions also extend smoothly through $\theta=k\pi$ and satisfy the original equation there. The two constants describe the general solution on any interval where the coordinate substitution is invertible.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [7](../../7.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
