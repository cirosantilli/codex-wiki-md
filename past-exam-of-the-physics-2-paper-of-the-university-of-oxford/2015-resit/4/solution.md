<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The magnetostatic [Ampère's law](../../../ampere-s-circuital-law.md) is $\oint\mathbf B\cdot d\boldsymbol\ell=\mu_0I_{\rm enc}$, equivalently $\nabla\times\mathbf B=\mu_0\mathbf J$ in vacuum. Let the wire radius be $a$ and take positive [electric current](../../../electric-current.md) along its axis. Cylindrical symmetry makes $\mathbf B$ azimuthal and constant in magnitude on a radius-$r$ circular path, so $2\pi rB=\mu_0I_{\rm enc}$.

Uniform [electric current](../../../electric-current.md) density gives $J=I/(\pi a^2)$. Inside the wire, $I_{\rm enc}=J\pi r^2=Ir^2/a^2$; outside, the full [electric current](../../../electric-current.md) is enclosed. Therefore

$$
\boxed{\mathbf B(r)=\begin{cases}
\dfrac{\mu_0Ir}{2\pi a^2}\hat{\boldsymbol\phi},&0\le r\le a,\\
\dfrac{\mu_0I}{2\pi r}\hat{\boldsymbol\phi},&r\ge a.
\end{cases}}
$$

The direction is set by the right-hand rule around the [electric current](../../../electric-current.md). The magnitude starts at zero on the axis, rises linearly to $\mu_0I/(2\pi a)$ at the surface and then falls as $1/r$. The two expressions are continuous at $r=a$. The long-wire approximation neglects end effects and any high-frequency redistribution of [electric current](../../../electric-current.md).

## ↑ Ancestors (11)

1. [4](../4.md)
2. [2015 resit](../../2015-resit-split.md)
3. [Past exam of the physics 2 paper of the University of Oxford](../../split.md)
4. [Physics 2 paper of the University of Oxford](../../../physics-2-paper-of-the-university-of-oxford.md)
5. [Year 1 of the physics course of the University of Oxford](../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
6. [Physics course of the University of Oxford](../../../physics-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../university-of-oxford-split.md)
10. [List of universities](../../../list-of-universities.md)
11. [Codex Wiki](../../../split.md)
