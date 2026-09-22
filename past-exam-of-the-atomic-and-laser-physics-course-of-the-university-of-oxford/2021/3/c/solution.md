<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For constant nonzero [absorption coefficient](../../../../absorption-coefficient.md), multiply the [radiative transfer equation](../../../../radiative-transfer-equation.md) by the [integrating factor](../../../../integrating-factor.md) $e^{\kappa_\nu z}$:

$$
\frac{d}{dz}(I_\nu e^{\kappa_\nu z})=j_\nu e^{\kappa_\nu z}.
$$

Integrating from the entrance to $z$ gives

$$
\boxed{I_\nu(z)=I_\nu(0)e^{-\kappa_\nu z}+S_\nu(1-e^{-\kappa_\nu z}),\qquad S_\nu=\frac{j_\nu}{\kappa_\nu}.}
$$

The boundary condition is immediate. Differentiation gives $I_\nu'=-\kappa_\nu[I_\nu(0)-S_\nu]e^{-\kappa_\nu z}=-\kappa_\nu I_\nu+j_\nu$, checking the equation. For positive [optical depth](../../../../optical-depth.md) $\kappa_\nu z\gg1$, the incident [specific intensity](../../../../spectral-radiance.md) is forgotten and $I_\nu\to S_\nu$. Negative [absorption coefficient](../../../../absorption-coefficient.md) instead describes gain and does not have this relaxation limit. At $\kappa_\nu=0$ use the nonsingular form directly: $I_\nu(z)=I_\nu(0)+j_\nu z$.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2021](../../../2021-split.md)
4. [Past exam of the atomic and laser physics course of the University of Oxford](../../../split.md)
5. [Atomic and laser physics course of the University of Oxford](../../../../atomic-and-laser-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
