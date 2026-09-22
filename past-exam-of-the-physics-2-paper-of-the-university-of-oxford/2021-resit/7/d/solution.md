<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use a [two-element radio interferometer](../../../../two-element-radio-interferometer.md): couple two small dishes coherently and align the projected baseline along the angular separation of the neighbouring satellites. Each dish's broad [antenna](../../../../antenna-radio.md) response should include both satellites. Match the electronic delays so that the desired satellite arrives in phase at the combiner. For baseline [length](../../../../length.md) $b$ perpendicular to the central line of sight, a small angular displacement $\theta$ produces geometric path difference $b\sin\theta$ and [phase difference](../../../../phase-difference.md)

$$
\phi(\theta)=\frac{2\pi b}{\lambda}\sin\theta.
$$

For equal signal [amplitudes](../../../../wave-amplitude.md) from one source, the output [wave intensity](../../../../intensity-physics.md) is $4I_0\cos^2(\phi/2)$. Put one satellite on a maximum and its neighbour on the first null: $\phi(\theta_R)=\pi$. The smallest useful projected baseline is therefore

$$
\boxed{b=\frac{\lambda}{2\sin\theta_R}\simeq\frac{\lambda}{2\theta_R}
=0.348\,\mathrm m.}
$$

The [angles](../../../../angle.md) here are measured near the normal to the baseline. At a general pointing angle $\theta_0$, replace $b$ in the small-separation estimate by $b\cos\theta_0$. Longer odd-half-fringe baselines can also null the neighbour but create more angular ambiguity. This arrangement provides discrimination along one direction; two collectors alone have repeated [interference fringes](../../../../interference-fringe.md) and do not produce an unambiguous full image.

## ↑ Ancestors (12)

1. [D](../d.md)
2. [7](../../7.md)
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
