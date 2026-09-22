<h1 id="9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Keep the same fixed laboratory equilibrium reference, and let the pivot move downward by $z(t)=z_0\cos\omega_0t$. The dynamic upper-spring extension is now $x_1-z$, so

$$
m\ddot{\mathbf x}+k\begin{pmatrix}2&-1\\-1&1\end{pmatrix}\mathbf x=k\begin{pmatrix}z(t)\\0\end{pmatrix}.
$$

At $\omega_0^2=k/m$, seek a particular solution $\mathbf x_p=\mathbf b\cos\omega_0t$. The amplitude equation is

$$
\begin{pmatrix}1&-1\\-1&0\end{pmatrix}\mathbf b=\begin{pmatrix}z_0\\0\end{pmatrix},\qquad \mathbf b=\begin{pmatrix}0\\-z_0\end{pmatrix}.
$$

Let $s_\pm=(3\pm\sqrt5)/2$, $\omega_\pm=\sqrt{ks_\pm/m}$ and $\mathbf u_\pm=(1-s_\pm,1)^{\mathsf T}$. The unrestricted general motion is

$$
\boxed{\mathbf x(t)=\sum_{\sigma=\pm}\mathbf u_\sigma[C_\sigma\cos\omega_\sigma t+D_\sigma\sin\omega_\sigma t]+\begin{pmatrix}0\\-z_0\cos\omega_0t\end{pmatrix}.}
$$

Four initial-condition constants are retained because none are specified. The driven particular response is not a resonance: $\omega_0$ differs from both eigenfrequencies. Its stationary upper mass is the [pivot-driven two-mass spring antiresonance](../../../../pivot-driven-two-mass-spring-antiresonance.md). Relative to the moving pivot, subtract $z(t)$ from both components.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [9](../../9.md)
3. [2014](../../../2014-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
