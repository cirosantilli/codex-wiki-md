# Spherical Abel deprojection

↑ **Parent:** [Spherical density projection](spherical-density-projection.md)

Put $F(u)=\Sigma(\sqrt u)$ and $g(v)=\rho(\sqrt v)$. Then $F(u)=\int_u^\infty g(v)/\sqrt{v-u}\,dv$. Composing this [Abel transform](abel-transform.md) with itself and exchanging convergent [integrals](integral.md) gives $\int_t^\infty F(u)/\sqrt{u-t}\,du=\pi\int_t^\infty g(v)\,dv$, because the inner integral from $t$ to $v$ is $\pi$. Differentiate after writing $u=t+s$ to obtain $g(t)=-\pi^{-1}\int_t^\infty F'(u)/\sqrt{u-t}\,du$. Substituting $t=r^2,u=R^2$ yields the displayed reconstruction. Decay and regularity sufficient for the exchanges and derivatives are required.

**Table of contents**

- [Power-law spherical projection kernel](power-law-spherical-projection-kernel.md)
- [Isotropic stellar pressure deprojection](isotropic-stellar-pressure-deprojection.md)

## ↑ Ancestors (8)

1. [Spherical density projection](spherical-density-projection.md)
2. [Stellar dynamics](stellar-dynamics.md)
3. [Galaxy dynamics](galaxy-dynamics.md)
4. [Galaxy](galaxy-split.md)
5. [Astrophysics](astrophysics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-40/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-40/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-73/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-62/1/solution.md)
