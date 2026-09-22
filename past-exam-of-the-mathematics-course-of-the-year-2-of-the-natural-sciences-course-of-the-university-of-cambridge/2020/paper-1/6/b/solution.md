<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Denote the unshifted differential expression by $L_0y=(py')'+qy$. The supplied [Green's function](../../../../../green-s-function-split.md) satisfies $L_0G(x,\xi)=\delta(x-\xi)$, whereas the inhomogeneous equation is $L_0y=\lambda wy+wf$.

Multiply the latter equation by $G$ and the Green equation by $y$, subtract and integrate in $x$:

$$
\int_a^b\left[G L_0y-yL_0G\right]dx
=\lambda\int_a^bwGy\,dx+\int_a^bwGf\,dx-y(\xi).
$$

The left-hand side is the boundary term

$$
\left[p(Gy'-yG_x)\right]_a^b.
$$

It vanishes because $G$ and $y$ satisfy the same homogeneous [Robin boundary conditions](../../../../../robin-boundary-condition.md). For example, where $\alpha\ne0$, substituting $y'=-\beta y/\alpha$ and $G_x=-\beta G/\alpha$ cancels the endpoint expression; where $\alpha=0$, both values vanish. The other endpoint works identically. Hence

$$
\boxed{\int_a^b f(x)w(x)G(x,\xi)\,dx
+\lambda\int_a^b w(x)G(x,\xi)y(x)\,dx-y(\xi)=0.}
$$

The [Dirac delta function](../../../../../dirac-delta-function.md) contribution is valid for an interior evaluation point $\xi$; equivalently, $G$ is continuous there and has flux-derivative jump $[pG_x]_{\xi^-}^{\xi^+}=1$.

This uses the existence of the unshifted [Green's function](../../../../../green-s-function-split.md) stated in the question. Such a function is not automatic for every choice of $p,q$ and endpoint conditions: a nontrivial [zero mode](../../../../../zero-mode.md) of $L_0$ would obstruct an ordinary inverse and would require a compatibility condition and a modified [Green's function](../../../../../green-s-function-split.md). Under the stated inverse assumption, the [differential equation](../../../../../differential-equation-split.md) and the displayed [integral equation](../../../../../integral-equation.md) are equivalent for functions in the boundary-condition domain.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
