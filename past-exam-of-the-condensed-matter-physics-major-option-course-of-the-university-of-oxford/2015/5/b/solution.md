<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the time dependence actually specified, $e^{i\omega t}$, and $\mathbf B=B\hat{\mathbf z}$. The component equations are

$$
(\tau^{-1}+i\omega)v_x=-\frac e{m^*}E_x-\omega_cv_y,\qquad
(\tau^{-1}+i\omega)v_y=-\frac e{m^*}E_y+\omega_cv_x,
\quad\omega_c=\frac{eB}{m^*}.
$$

Adding the second equation multiplied by $\pm i$ diagonalizes the response. With the literal definitions $v_\pm=v_x\pm iv_y$, $E_\pm=E_x\pm iE_y$, and $J_\pm=-ne v_\pm$,

$$
\boxed{\sigma_\pm=\frac{ne^2/m^*}{\tau^{-1}+i(\omega\mp\omega_c)}
=\frac{\sigma_0}{1+i(\omega\mp\omega_c)\tau},\qquad\sigma_0=\frac{ne^2\tau}{m^*}.}
$$

**The source's printed $\omega\pm\omega_c$ reverses the helicity labels for these definitions.** It is recovered by naming the two circular components oppositely, reversing $B$, or changing the matching time/[polarization](../../../../polarization-waves.md) convention. As a concrete check, with $E_+\ne0$, $E_-=0$ and positive $B$, the collisionless component equation resonates at $\omega=\omega_c$. The printed plus-labeled denominator would instead remain proportional to $2i\omega_c$. The physical result is unambiguous: only the [circular polarization](../../../../circular-polarization.md) rotating with the electron orbit has positive-frequency [cyclotron resonance](../../../../cyclotron-resonance.md).

For the convention used here, the dielectric eigenvalues are $\epsilon_\pm=\epsilon_\infty+\sigma_\pm/(i\epsilon_0\omega)$. In the lossless limit,

$$
\boxed{\epsilon_\pm=\epsilon_\infty-\frac{\omega_p^2}{\omega(\omega\mp\omega_c)},\qquad
\omega_p^2=\frac{ne^2}{\epsilon_0m^*}.}
$$

These eigenvalues determine propagation and reflection in the Faraday geometry; changing the helicity names swaps their subscripts without changing any optical prediction.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics major option course of the University of Oxford](../../../split.md)
5. [Condensed matter physics major option course of the University of Oxford](../../../../condensed-matter-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
