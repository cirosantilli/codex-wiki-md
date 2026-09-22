<h1 id="8/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let the original cylinder axis be $\mathbf r=\mathbf0$, and let the hole axis be at transverse [vector](../../../../vector.md) $\mathbf a$, with $|\mathbf a|=a$. The [charge density](../../../../charge-density.md) is reproduced by a full cylinder of [radius](../../../../radius.md) $R_1$ and [charge density](../../../../charge-density.md) $+\rho$, superposed with a cylinder of [radius](../../../../radius.md) $R_2$ centred at $\mathbf a$ and [charge density](../../../../charge-density.md) $-\rho$. This uses the [superposition principle](../../../../superposition-principle.md) for fixed insulating [electric charges](../../../../electric-charge-split.md); the hole is not a hole in an [electrical conductor](../../../../electrical-conductor.md).

For a complete uniformly charged infinite cylinder of [radius](../../../../radius.md) $R$, a coaxial [Gaussian surface](../../../../gaussian-surface.md) of [length](../../../../length.md) $\ell$ gives, by [Gauss's law](../../../../gauss-s-law.md),

$$
2\pi s\ell E(s)=\begin{cases}\rho\pi s^2\ell/\epsilon_0,&s<R,\\
\rho\pi R^2\ell/\epsilon_0,&s\geq R.
\end{cases}
$$

Consequently define

$$
\mathbf F_R(\mathbf s)=\begin{cases}\mathbf s,&|\mathbf s|\leq R,\\
R^2\mathbf s/|\mathbf s|^2,&|\mathbf s|>R.
\end{cases}
$$

The complete [electric field](../../../../electric-field-split.md), including the exterior if desired, is

$$
\boxed{\mathbf E(\mathbf r)=\frac\rho{2\epsilon_0}
\left[\mathbf F_{R_1}(\mathbf r)-\mathbf F_{R_2}(\mathbf r-\mathbf a)\right].}
$$

In the insulating material, $|\mathbf r|<R_1$ and $s=|\mathbf r-\mathbf a|>R_2$, so

$$
\boxed{\mathbf E_{\rm material}(\mathbf r)=\frac\rho{2\epsilon_0}
\left[\mathbf r-\frac{R_2^2(\mathbf r-\mathbf a)}{|\mathbf r-\mathbf a|^2}\right].}
$$

Inside the hole both contributions use their interior formulas, and all dependence on $\mathbf r$ cancels:

$$
\boxed{\mathbf E_{\rm hole}=\frac\rho{2\epsilon_0}[\mathbf r-(\mathbf r-\mathbf a)]
=\frac\rho{2\epsilon_0}\mathbf a.}
$$

The [electric field](../../../../electric-field-split.md) in the hole is uniform, points from the original axis towards the hole axis for $\rho>0$, and vanishes for a concentric hole. The two expressions agree at the hole wall, as expected with no imposed [surface charge density](../../../../surface-charge-density.md) there. Its uniformity is the useful [uniform electric field in an off-axis cylindrical cavity](../../../../uniform-electric-field-in-an-off-axis-cylindrical-cavity.md) result.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [8](../../8.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the physics 2 paper of the University of Oxford](../../../split.md)
5. [Physics 2 paper of the University of Oxford](../../../../physics-2-paper-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
