<h1 id="differential-equations/9/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Write $\omega=\sqrt2$ and $Y(p)=\overline y(p)$. The zero initial data and the [Laplace transform of a derivative](../../../../../laplace-transform-of-a-derivative.md) give $\mathcal L[y'']=p^2Y$. Transforming the forcing with part (b),

$$
\begin{aligned}
(p^2+2)Y
&=\sqrt2\,\frac{p^2-2}{(p^2+2)^2}
+\frac12\frac{\sqrt2}{p^2+2}\\
&=\frac{\sqrt2(3p^2-2)}{2(p^2+2)^2}.
\end{aligned}
$$

Therefore

$$
\boxed{Y(p)=\frac{\sqrt2(6p^2-4)}{4(p^2+2)^3}.}
$$

Part (b) with $\omega=\sqrt2$ gives $\mathcal L[t^2\sin(\sqrt2t)]=2\sqrt2(3p^2-2)/(p^2+2)^3$. Comparing coefficients and using uniqueness of the [Laplace transform](../../../../../laplace-transform.md),

$$
\boxed{y(t)=\frac{t^2}{4}\sin(\sqrt2\,t).}
$$

As a direct check, $y'=\tfrac t2\sin(\sqrt2t)+\tfrac{\sqrt2t^2}4\cos(\sqrt2t)$, so both initial values vanish. Differentiating once more cancels the $t^2\sin(\sqrt2t)$ terms in $y''+2y$, leaving $\sqrt2t\cos(\sqrt2t)+\tfrac12\sin(\sqrt2t)$ as required. This also checks the factor $1/4$ in the inverse transform.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [9](../../9.md)
3. [Differential Equations](../../../differential-equations.md)
4. [2013](../../../../2013-split.md)
5. [Past exam of the algebra, analysis and differential equations 1 course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations 1 course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-1-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
