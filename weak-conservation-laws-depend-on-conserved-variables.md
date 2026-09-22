# Weak conservation laws depend on conserved variables

↑ **Parent:** [System of conservation laws](system-of-conservation-laws.md)

Two smooth differential systems related by a nonlinear change of dependent variables need not define the same [weak solutions](weak-solution.md). If $U_t+F(U)_x=0$, a smooth function $V=g(U)$ satisfies $V_t+g'(U)F'(U)U_x=0$ for smooth $U$; even when this can be written as another divergence, its [Rankine-Hugoniot conditions](rankine-hugoniot-conditions.md) need not be equivalent to those in $U$. The smooth chain rule does not justify multiplying jump distributions by discontinuous coefficients.

For example the [shallow water equations](shallow-water-equations.md) can be written smoothly as $h_t+(hv)_x=0$ and $v_t+(h+v^2/2)_x=0$. Mechanical mass and [momentum conservation](momentum-conservation.md) instead select $h_t+(hv)_x=0$ and $(hv)_t+(hv^2+h^2/2)_x=0$. These systems agree for smooth positive $h$, but their jump laws differ. The states $(h,v)=(2,\sqrt3/2)$ and $(1,0)$ satisfy the mass/momentum jump laws with speed $\sqrt3$, while the velocity-form jump equation would demand $11/(4\sqrt3)$. A model for discontinuities must specify the conservative variables or an equivalent admissible regularization, rather than using smooth equivalence alone.

## ↑ Ancestors (7)

1. [System of conservation laws](system-of-conservation-laws.md)
2. [Transport equation](transport-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2010/b/5/b/i/solution.md)
