# Newton cooling with an instantaneous temperature jump

↑ **Parent:** [Newton's law of cooling](newton-s-law-of-cooling.md)

Under [Newton's law of cooling](newton-s-law-of-cooling.md) with fixed ambient temperature $T_0$ and $k>0$, an instantaneous jump $\beta$ at $t_*$ sets $T(t_*+)=T(t_*-)+\beta$. The subsequent temperature is $T_0+[T(t_*-)+\beta-T_0]e^{-k(t-t_*)}$. Equivalently, for an initial temperature $T_i$, the full solution is

$$
T(t)=T_0+(T_i-T_0)e^{-kt}+\beta H(t-t_*)e^{-k(t-t_*)}.
$$

This piecewise model has the [distributional derivative](distributional-derivative.md) equation $T'+k(T-T_0)=\beta\delta(t-t_*)$, with the [Dirac delta distribution](dirac-delta-function.md) representing the added temperature.

## ↑ Ancestors (8)

1. [Newton's law of cooling](newton-s-law-of-cooling.md)
2. [Linear ordinary differential equation](linear-ordinary-differential-equation.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ia/paper-2/5a/b/ii/solution.md)
