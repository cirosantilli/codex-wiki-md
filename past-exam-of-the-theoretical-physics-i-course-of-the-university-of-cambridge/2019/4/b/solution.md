<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The stationary points of the [Landau free energy](../../../../landau-free-energy.md) obey

$$
f'(m)=2m(r+bm^2+cm^4)=0.
$$

For $b>0$, $r\geq0$ makes every term of $f$ nonnegative, so $m=0$ is the unique [global minimum](../../../../global-minimum.md). For $r<0$, its curvature $f''(0)=2r$ is negative. Setting $x=m^2$ gives $cx^2+bx+r=0$, whose unique positive root is

$$
x_+=\frac{-b+\sqrt{b^2-4cr}}{2c}.
$$

At a nonzero stationary point,

$$
f''(m)=4x(b+2cx),\qquad f(m)=-\frac b2x^2-\frac{2c}{3}x^3.
$$

Thus both $m=\pm\sqrt{x_+}$ are stable and have lower [free energy](../../../../thermodynamic-free-energy.md) than $m=0$. The [equilibrium magnetization](../../../../equilibrium-magnetization.md) is

$$
\boxed{m_{\rm eq}=\begin{cases}
0,&T\geq T_c,\\
\displaystyle\pm\left[\frac{-b+\sqrt{b^2+4ac(T_c-T)}}{2c}\right]^{1/2},&T<T_c.
\end{cases}}
$$

For fixed $b>0$ and $T\to T_c^-$, expand the square root:

$$
m_{\rm eq}^2=\frac{a(T_c-T)}b+O((T_c-T)^2).
$$

It tends continuously to zero. Hence the [continuous phase transition](../../../../continuous-phase-transition.md) has the [order-parameter critical exponent](../../../../order-parameter-critical-exponent.md)

$$
\boxed{|m_{\rm eq}|\sim\sqrt{\frac ab}(T_c-T)^{1/2},\qquad\beta=\frac12.}
$$

This is the [mean-field critical exponent](../../../../mean-field-critical-exponent.md); fluctuation corrections beyond [Landau theory](../../../../landau-theory.md) are not included.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [4](../../4.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the theoretical physics I course of the University of Cambridge](../../../split.md)
5. [Theoretical Physics I course of the University of Cambridge](../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
6. [Theoretical Physics course of the University of Cambridge](../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../list-of-universities.md)
14. [Codex Wiki](../../../../split.md)
