# Salt-rejection function for a saline Stefan front

↑ **Parent:** [Saline Stefan problem](saline-stefan-problem.md)

For salt-free [ice](ice.md) and a liquid [concentration](concentration.md) profile proportional to $\operatorname{erfc}[x/(2\sqrt{Dt})]$, [salt rejection](salt-rejection.md) at $a=2\lambda\sqrt{Dt}$ gives $C_iF(\lambda)=C_0$, where $D$ is the salt [diffusion coefficient](diffusion-coefficient.md), and $C_i,C_0$ are the interface and far-field [concentrations](concentration.md). This follows from $-DC_x(a^+)=\dot a C_i$. The function is positive and strictly decreasing for all real $\lambda$, since an integration by parts gives

$$
F(\lambda)=2\int_0^\infty u e^{-u^2-2\lambda u}\,du,\qquad F'(\lambda)=-4\int_0^\infty u^2e^{-u^2-2\lambda u}\,du<0.
$$

Consequently $C_i=C_0/F(\lambda)$ increases with $\lambda$, equals $C_0$ at zero, and is enriched for freezing and diluted for melting. The positivity proof also prevents spurious negative interface [concentrations](concentration.md) when using the [complementary error function](complementary-error-function.md) formula.

## ↑ Ancestors (7)

1. [Saline Stefan problem](saline-stefan-problem.md)
2. [Stefan problem](stefan-problem.md)
3. [Planetary ice shell](planetary-ice-shell.md)
4. [Geophysics](geophysics-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-332/2/solution.md)
- [Small-diffusivity constitutional-supercooling threshold](small-diffusivity-constitutional-supercooling-threshold.md)
