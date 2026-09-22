<h1 id="6/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [lepton mixing matrix](../../../../lepton-mixing-matrix.md) is [unitary](../../../../unitary-connection.md), so each row has unit norm. Explicitly its electron row obeys

$$
|U_{e1}|^2+|U_{e2}|^2+|U_{e3}|^2
=c_{13}^2(c_{12}^2+s_{12}^2)+s_{13}^2=1,
$$

where $c_{ij}=\cos\theta_{ij}$ and $s_{ij}=\sin\theta_{ij}$. This is also the normalization needed for unit [electron neutrino](../../../../electron-neutrino.md) survival at $L=0$.

Use $\operatorname{Re}(1-e^{ix})=1-\cos x=2\sin^2(x/2)$ and define $\Delta_{ij}=(\phi_i-\phi_j)/2=\Delta m_{ij}^2L/(4E)$ in [natural units](../../../../natural-units.md). The exact vacuum [neutrino oscillation](../../../../neutrino-oscillation.md) result becomes

$$
P_{ee}=1-4\sum_{i<j}|U_{ei}|^2|U_{ej}|^2\sin^2\Delta_{ij}.
$$

The given [mass-squared differences](../../../../mass-squared-difference.md) satisfy $|\Delta m_{12}^2/\Delta m_{23}^2|\simeq0.027\ll1$, so the two fast [oscillation](../../../../oscillation.md) frequencies are close: $\Delta_{13}=\Delta_{23}+\Delta_{12}$. Approximating their phases as equal combines their coefficients into

$$
4s_{13}^2c_{13}^2(c_{12}^2+s_{12}^2)=\sin^22\theta_{13},
$$

while $4c_{12}^2s_{12}^2c_{13}^4=c_{13}^4\sin^22\theta_{12}$. Hence

$$
\boxed{P_{ee}\simeq1-\cos^4\theta_{13}\sin^22\theta_{12}\sin^2\Delta_{12}
-\sin^22\theta_{13}\sin^2\Delta_{23}.}
$$

The complex [CP](../../../../cp-symmetry.md) phase cancels from every $|U_{ei}|^2$. The phase-replacement approximation is uniformly reliable for $|\Delta_{12}|\ll1$, especially at short reactor baselines; closeness of the [mass-squared differences](../../../../mass-squared-difference.md) alone does not guarantee close sine values at arbitrarily large $L/E$. At medium baselines the distinct fast frequencies can beat, so the exact three-frequency expression is preferable if their detailed pattern matters.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [6](../../6.md)
3. [2022](../../../2022-split.md)
4. [Past exam of the particle physics course of the University of Oxford](../../../split.md)
5. [Particle physics course of the University of Oxford](../../../../particle-physics-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
