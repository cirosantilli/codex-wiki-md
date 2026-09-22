# Erlang claim-size differential equation for survival probability

↑ **Parent:** [Survival integro-differential equation for a classical risk model](survival-integro-differential-equation-for-a-classical-risk-model.md)

For an [Erlang distribution](erlang-distribution.md) claim density $f(x)=\beta^2xe^{-\beta x}$ and $r=\lambda/c$, write $H=\phi*f$. The [survival integro-differential equation](survival-integro-differential-equation-for-a-classical-risk-model.md) gives $\phi'=r(\phi-H)$. The convolution satisfies $(D+\beta)^2H=\beta^2\phi$, because $H=\beta^2e^{-\beta u}\int_0^u(u-t)\phi(t)e^{\beta t}dt$. Applying $(D+\beta)^2$ to the first equation eliminates $H$ and gives the displayed third-order equation. The original integral equation also supplies $\phi'(0)=r\phi(0)$ and $\phi''(0)=r^2\phi(0)$; these conditions must not be lost when solving the higher-order equation.

## ↑ Ancestors (8)

1. [Survival integro-differential equation for a classical risk model](survival-integro-differential-equation-for-a-classical-risk-model.md)
2. [Survival renewal equation for a classical risk model](survival-renewal-equation-for-a-classical-risk-model.md)
3. [Classical risk model](classical-risk-model.md)
4. [Actuarial statistics](actuarial-statistics-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-37/3/solution.md)
