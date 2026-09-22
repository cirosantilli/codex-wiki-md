<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use [Gaussian units](../../../../gaussian-units.md), [plane waves](../../../../plane-wave.md) proportional to $e^{i\mathbf k\cdot\mathbf r-i\omega t}$, and the **signed** [cyclotron frequency](../../../../cyclotron-frequency.md) $\Omega_s=q_sB_0/(m_sc)$. Write $\Omega_e=eB_0/(m_ec)>0$ for its [electron](../../../../electron.md) magnitude, so the signed [electron](../../../../electron.md) value is $-\Omega_e$. Define the species [plasma frequency](../../../../plasma-frequency.md) by $\omega_{ps}^2=4\pi n_{0s}q_s^2/m_s$. The [linearization](../../../../linearization.md) of the cold [Lorentz force](../../../../lorentz-force.md) equations gives

$$
-i\omega u_{xs}-\Omega_su_{ys}=\frac{q_s}{m_s}E_x,\qquad
\Omega_su_{xs}-i\omega u_{ys}=\frac{q_s}{m_s}E_y,\qquad
-i\omega u_{zs}=\frac{q_s}{m_s}E_z.
$$

Solving this [linear system](../../../../system-of-linear-equations.md) and using the species [current density](../../../../current-density.md) $\mathbf j_s=n_{0s}q_s\mathbf u_s$ gives the [conductivity tensor](../../../../conductivity-tensor.md)

$$
\boxed{\boldsymbol\sigma_s=\frac{n_{0s}q_s^2}{m_s}
\begin{pmatrix}
\dfrac{i\omega}{\omega^2-\Omega_s^2}&-\dfrac{\Omega_s}{\omega^2-\Omega_s^2}&0\\
\dfrac{\Omega_s}{\omega^2-\Omega_s^2}&\dfrac{i\omega}{\omega^2-\Omega_s^2}&0\\
0&0&\dfrac{i}{\omega}
\end{pmatrix}.}
$$

The [magnetized cold-plasma dielectric tensor](../../../../magnetized-cold-plasma-dielectric-tensor.md) is $\boldsymbol\epsilon=\mathbf I+(4\pi i/\omega)\sum_s\boldsymbol\sigma_s$. Thus

$$
\boldsymbol\epsilon=\begin{pmatrix}S&ig&0\\-ig&S&0\\0&0&P\end{pmatrix},\quad
S=\epsilon_\perp=1-\sum_s\frac{\omega_{ps}^2}{\omega^2-\Omega_s^2},\quad
P=\epsilon_\parallel=1-\sum_s\frac{\omega_{ps}^2}{\omega^2},\quad
g=-\sum_s\frac{\omega_{ps}^2\Omega_s}{\omega(\omega^2-\Omega_s^2)}.
$$

At the stated [electron](../../../../electron.md) [frequency](../../../../frequency.md) scale, the [ion](../../../../ion.md) contribution is smaller by $O(Zm_e/m_i)$ for $q_i=Ze$ and [quasineutrality](../../../../quasineutrality.md). To this accuracy,

$$
\boxed{S=1-\frac{\omega_{pe}^2}{\omega^2-\Omega_e^2},\qquad
P=1-\frac{\omega_{pe}^2}{\omega^2},\qquad
g=\frac{\omega_{pe}^2\Omega_e}{\omega(\omega^2-\Omega_e^2)}.}
$$

These expressions require negligible [collisions](../../../../collision.md) and the cold ordering $kv_{\mathrm{th},s}\ll|\omega|$; sufficiently close to a [cyclotron resonance](../../../../cyclotron-resonance.md), thermal broadening or [collisions](../../../../collision.md) must also be retained.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the collisionless plasma physics course of the University of Oxford](../../../split.md)
5. [Collisionless plasma physics course of the University of Oxford](../../../../collisionless-plasma-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
