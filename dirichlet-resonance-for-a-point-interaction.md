# Dirichlet resonance for a point interaction

↑ **Parent:** [Point interaction in a second-order differential equation](point-interaction-in-a-second-order-differential-equation.md)

The [boundary value problem](boundary-value-problem-split.md) $y''+\alpha y(c)\delta_c=f$ on $(0,\ell)$ with [Dirichlet boundary conditions](dirichlet-boundary-condition.md) has a unique solution for every continuous forcing and prescribed endpoint values exactly when $\alpha\ne\alpha_*:=\ell/(c(\ell-c))$. The left-normalized homogeneous solution is

$$
u_\alpha(x)=x-\alpha c(x-c)_+,\qquad u_\alpha(\ell)=\ell-\alpha c(\ell-c),
$$

where $(t)_+=\max(t,0)$. Continuity at $c$ and the [transmission conditions for a delta coefficient](transmission-conditions-for-a-delta-coefficient.md) give this formula. The final boundary condition fixes the initial slope unless the displayed endpoint value is zero. This is a one-dimensional [kernel](kernel-of-a-linear-map-split.md) obstruction, analogous to the [Fredholm alternative](fredholm-alternative.md).

At resonance the normalized null function is

$$
\phi(x)=\begin{cases}x/c,&0\leq x\leq c,\\(\ell-x)/(\ell-c),&c\leq x\leq\ell.\end{cases}
$$

For $y(0)=a$ and $y(\ell)=b$, the compatibility condition is

$$
\int_0^\ell\phi(x)f(x)\,dx=\frac ac+\frac b{\ell-c}.
$$

Indeed, integrate $\phi L_\alpha y-yL_\alpha\phi$ on both sides of $c$. The internal terms cancel by the matching derivative jumps, leaving $[\phi y'-\phi'y]_0^\ell$. This equals the right-hand side. The initial-slope construction also proves sufficiency: when compatible there is a one-parameter family $y_0+t\phi$; otherwise no solution exists.

## ↑ Ancestors (9)

1. [Point interaction in a second-order differential equation](point-interaction-in-a-second-order-differential-equation.md)
2. [Second-order linear differential equation](second-order-linear-differential-equation.md)
3. [Linear ordinary differential equation](linear-ordinary-differential-equation-split.md)
4. [Ordinary differential equation](ordinary-differential-equation.md)
5. [Differential equation](differential-equation-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Dirichlet Green function for a point interaction](dirichlet-green-function-for-a-point-interaction.md)
- [Solution](past-exam-of-the-differential-equations-2-course-of-the-university-of-oxford/2017/1/b/i/solution.md)
