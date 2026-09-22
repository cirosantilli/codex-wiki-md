# Reflected-step solution of the wave equation

↑ **Parent:** [Wave equation](wave-equation-split.md)

For $y_{tt}=c^2y_{xx}$ on $0<x<L$, initially at rest with zero displacement, apply $y(0,t)=a$ for $t>0$ and keep $y(L,t)=0$. A [geometric series](geometric-series.md) in the [Laplace transform](laplace-transform.md) gives

$$
y(x,t)=a\sum_{m\geq0}\left[H\!\left(t-\frac{2mL+x}{c}\right)-H\!\left(t-\frac{(2m+2)L-x}{c}\right)\right].
$$

Here $H$ is the [Heaviside step function](heaviside-step-function.md), $L,c>0$, and only finitely many terms contribute at any finite time. The second step in each pair is a sign-reversed reflection from the fixed endpoint. The formula solves the [wave equation](wave-equation-split.md) classically away from the fronts and distributionally across them; the midpoint is a square wave of period $2L/c$.

## ↑ Ancestors (6)

1. [Wave equation](wave-equation-split.md)
2. [Partial differential equation](partial-differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/ib/paper-4/14a/c/ii/solution.md)
