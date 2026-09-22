<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [cylindrical coordinate system](../../../../cylindrical-coordinate-system.md) basis $\mathbf e_r,\mathbf e_\varphi,\mathbf e_z$. The meridional unit [tangent vector](../../../../tangent-vector-split.md) and outward unit [normal vector](../../../../normal-vector.md) consistent with the given geometry are

$$
\mathbf e_s=\cos\theta\,\mathbf e_r-\sin\theta\,\mathbf e_z,
\qquad
\mathbf n=\sin\theta\,\mathbf e_r+\cos\theta\,\mathbf e_z.
$$

An [surface of revolution](../../../../surface-of-revolution.md) has $\theta$ independent of $\varphi$. Consequently

$$
\partial_s\mathbf e_s=-\theta_s\mathbf n,\qquad
\partial_\varphi\mathbf e_\varphi=-\mathbf e_r,
\qquad
\mathbf e_r=\cos\theta\,\mathbf e_s+\sin\theta\,\mathbf n.
$$

Apply the [product rule](../../../../product-rule.md) to the vector [force balance](../../../../force-balance.md):

$$
\begin{aligned}
\partial_s(rt_s\mathbf e_s)
&=(r_s t_s+r\partial_s t_s)\mathbf e_s-rt_s\theta_s\mathbf n,\\
\partial_\varphi(t_\varphi\mathbf e_\varphi)
&=(\partial_\varphi t_\varphi)\mathbf e_\varphi
-t_\varphi\cos\theta\,\mathbf e_s-t_\varphi\sin\theta\,\mathbf n.
\end{aligned}
$$

Equating the three independent components to zero, and using $r_s=\cos\theta$, gives

$$
\begin{aligned}
\mathbf e_s &: \quad r\partial_s t_s+(t_s-t_\varphi)\cos\theta=0,\\
\mathbf e_\varphi &: \quad \partial_\varphi t_\varphi=0,\\
\mathbf n &: \quad rP-rt_s\theta_s-t_\varphi\sin\theta=0.
\end{aligned}
$$

Thus, away from the rotation axis where $r>0$, the scalar [mechanical equilibrium](../../../../mechanical-equilibrium.md) equations are

$$
\boxed{P=t_s\theta_s+t_\varphi\frac{\sin\theta}{r},\qquad
\partial_s t_s=\frac{\cos\theta}{r}(t_\varphi-t_s),\qquad
\partial_\varphi t_\varphi=0.}
$$

The two geometric factors $\theta_s$ and $\sin\theta/r$ are the signed meridional and azimuthal [principal curvatures](../../../../principal-curvature.md) in this convention. The normal equation is the [Young–Laplace equation](../../../../young-laplace-equation.md) generalized to unequal principal [membrane tensions](../../../../membrane-tension.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the mathematical mechanical biology course of the University of Oxford](../../../split.md)
5. [Mathematical mechanical biology course of the University of Oxford](../../../../mathematical-mechanical-biology-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
