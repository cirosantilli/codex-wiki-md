# Time reparametrization for a separable conservation-law flux

↑ **Parent:** [Scalar conservation law](scalar-conservation-law.md)

Suppose $a(t)>0$ for positive times. The strictly increasing new time $T(t)=\int_0^t a(s)\,ds$ converts the [scalar conservation law](scalar-conservation-law.md) $u_t+a(t)\partial_xF(u)=0$ into $U_T+\partial_xF(U)=0$, with $u(x,t)=U(x,T(t))$. The [chain rule](chain-rule.md) proves the claim for classical solutions; a change of variables in the weak formulation proves it for [weak solutions](weak-solution.md) and preserves the time orientation of the [Kruzhkov entropy inequality](kruzhkov-entropy-inequality.md). An isolated zero of $a$ at the initial endpoint does not obstruct the positive-time transformation.

The [Rankine-Hugoniot condition](rankine-hugoniot-conditions.md) becomes $dx_s/dt=a(t)[F(u)]/[u]$, while [characteristic curves](characteristic-curve.md) obey $dx/dt=a(t)F'(u)$. Thus a straight [shock](shock-wave.md) in the new time may accelerate in physical time. For $a(t)=t$, a constant-speed trajectory in $T=t^2/2$ is a parabola in $(x,t)$. This separates genuine changes in wave structure from a common time-dependent speed factor.

## ↑ Ancestors (7)

1. [Scalar conservation law](scalar-conservation-law.md)
2. [Transport equation](transport-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-differential-equations-and-applications-course-of-the-university-of-oxford/2008/a/4/a/ii/solution.md)
