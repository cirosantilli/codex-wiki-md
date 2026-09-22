# Expanding-flow transformation of a wave equation

↑ **Parent:** [Characteristic coordinate](characteristic-coordinate.md)

The change of variables $X=\rho e^{-t}$, $S=e^{-t}>0$ turns

$$
u_{tt}-\partial_\rho((1-\rho^2)u_\rho)+\partial_\rho(\rho u_t)+\rho u_{\rho t}=0
$$

into $w_{SS}-w_{XX}=0$. Indeed, with $D=\partial_t+\rho\partial_\rho$, the original operator is $D^2+D-\partial_\rho^2$, while $D=-S\partial_S$ and $\partial_\rho=S\partial_X$. Its [characteristic curves](characteristic-curve.md) are $\rho=-1+Ce^t$ and $\rho=1+Ce^t$, including the characteristic lines $\rho=\pm1$. General smooth solutions have the form $F(e^{-t}(\rho+1))+G(e^{-t}(\rho-1))$. Zero [Cauchy data](cauchy-data.md) on $-1<\rho<1$ at $t=0$ force vanishing throughout that strip for $t\geq0$, but not for all negative time: $u=(e^{-t}(\rho+1)-2)_+^3$ is a global $C^2$ counterexample. Thus the characteristic barriers describe a forward domain of dependence, not a barrier in both time directions.

## ↑ Ancestors (9)

1. [Characteristic coordinate](characteristic-coordinate.md)
2. [Characteristic hypersurface](characteristic-hypersurface.md)
3. [Principal symbol of a partial differential equation](principal-symbol-of-a-partial-differential-equation.md)
4. [Quasilinear partial differential equation](quasilinear-partial-differential-equation.md)
5. [Partial differential equation](partial-differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/4/b/ii/solution.md)
