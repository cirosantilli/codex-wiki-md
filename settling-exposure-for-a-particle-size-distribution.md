# Settling exposure for a particle size distribution

↑ **Parent:** [Axisymmetric settling box model](axisymmetric-settling-box-model.md)

In a mixed [particle-laden gravity current](particle-laden-gravity-current.md), a size class with settling speed $w$ has concentration $c(w,t)=c_0(w)e^{-wJ(t)}$. The shared [reduced gravity](reduced-gravity-split.md) is $g'(J)=\int g_0(w)c_0(w)e^{-wJ}\,dw$, and $dR^4/dJ=4\operatorname{Fr}(\mathcal V/\pi)^{3/2}\sqrt{g'(J)}$. Finite runout therefore requires $\int_0^\infty\sqrt{g'(J)}\,dJ<\infty$. A positive minimum settling speed guarantees this; a distribution with arbitrarily small settling speeds need not. For $g_0c_0(w)\sim Cw^p$ at zero, with $p>-1$, the integral converges precisely when $p>1$.

## ↑ Ancestors (9)

1. [Axisymmetric settling box model](axisymmetric-settling-box-model.md)
2. [Particle-laden gravity current](particle-laden-gravity-current.md)
3. [Gravity-current box model](gravity-current-box-model.md)
4. [Gravity current](gravity-current.md)
5. [Reduced gravity](reduced-gravity-split.md)
6. [Fluid mechanics](fluid-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-83/3/ii/solution.md)
