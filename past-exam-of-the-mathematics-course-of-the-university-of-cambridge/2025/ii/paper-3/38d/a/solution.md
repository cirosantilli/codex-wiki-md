<h1 id="38d/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The incompressibility equation turns the advective term into a divergence:

$$
u u_x+v u_y=\partial_x(u^2)+\partial_y(uv),
$$

because $v_y=-u_x$. For a plume in an otherwise stationary environment, the boundary-layer pressure equals the ambient pressure and has no imposed $x$-gradient. Integrating the vertical momentum equation across $y$ therefore gives

$$
\frac{d}{dx}\int_{-\infty}^{\infty}\rho u^2\,dy
+[\rho uv]_{-\infty}^{\infty}
=\mu[u_y]_{-\infty}^{\infty}+b(x).
$$

Both boundary terms vanish as the velocity and shear decay away from the plume. Hence the [integral momentum-flux balance for a two-dimensional plume](../../../../../../integral-momentum-flux-balance-for-a-two-dimensional-plume.md) is

$$
\boxed{\frac{d}{dx}\int_{-\infty}^{\infty}\rho u^2\,dy=b(x)}.
$$

## ↑ Ancestors (11)

1. [A](../a.md)
2. [38D](../../38d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
