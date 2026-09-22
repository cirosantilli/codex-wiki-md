<h1 id="k/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Writing $z=re^{i\theta}$ gives $\phi=\Gamma\theta/(2\pi)$ and $\psi=-\Gamma\log r/(2\pi)$. Constant [streamfunction](../../../../stream-function.md) means constant radius, so streamlines are circles. The tangential velocity is $v_\theta=\Gamma/(2\pi r)$, and its anticlockwise [circulation](../../../../circulation-physics.md) is $\int_0^{2\pi}v_\theta r\,d\theta=\Gamma$.

Use an opposite vortex at $z=-1$ as the image of the vortex at one:

$$
\boxed{w(z)=-\frac{i\Gamma}{2\pi}[\log(z-1)-\log(z+1)].}
$$

On $z=iy$ the two distances are equal, so $\psi=0$ and the wall is a [streamline](../../../../streamline.md). Its velocity follows from $w'=-i\Gamma/[\pi(z^2-1)]$: at the wall $u=0$ and $v=-\Gamma/[\pi(1+y^2)]$.

The [Bernoulli equation](../../../../bernoulli-equation.md) gives $p-p_\infty=-\rho\Gamma^2/[2\pi^2(1+y^2)^2]$. Relative to the ambient pressure force, the fluid's excess force on the wall is $-\int(p-p_\infty)dy$ in the positive $x$ direction. Using the supplied integral,

$$
\boxed{\mathbf F_{\rm vortex}=\frac{\rho\Gamma^2}{4\pi}\,\mathbf e_x\quad\text{per unit width}.}
$$

Thus the wall is attracted toward the fluid and vortex. Subtracting the uniform ambient pressure isolates the finite force due to the vortex.

## ↑ Ancestors (12)

1. [2](../2.md)
2. [K](../../k.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the probability, statistics and options I course of the University of Oxford](../../../split.md)
5. [Probability, statistics and options I course of the University of Oxford](../../../../probability-statistics-and-options-i-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics and statistics course of the University of Oxford](../../../../year-2-of-the-mathematics-and-statistics-course-of-the-university-of-oxford.md)
7. [Mathematics and statistics course of the University of Oxford](../../../../mathematics-and-statistics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
