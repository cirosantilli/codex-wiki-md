# Quadratic profiles for nonlinear diffusion with constant loss

↑ **Parent:** [Nonlinear diffusion equation](nonlinear-diffusion-equation.md)

For the displayed [nonlinear diffusion equation](nonlinear-diffusion-equation.md), a quadratic ansatz $h=A(t)+B(t)x^2$ reduces the [partial differential equation](partial-differential-equation-split.md) exactly to

$$
B'=6B^2,\qquad A'=2AB-1.
$$

Indeed $(hh_x)_x=2AB+6B^2x^2$, and equality of the constant and quadratic [coefficients](coefficient.md) proves the reduction. For nonzero curvature, integration gives $B=-1/[6(t-t_0)]$. On $\tau=t-t_0>0$, the remaining [linear ordinary differential equation](linear-ordinary-differential-equation-split.md) is $A'+A/(3\tau)=-1$, whose [integrating factor](integrating-factor.md) is $\tau^{1/3}$. Thus, including spatial translation,

$$
h(x,t)=C\tau^{-1/3}-\frac{(x-x_0)^2}{6\tau}-\frac34\tau.
$$

All three constants $C,x_0,t_0$ are arbitrary, on a domain with $\tau>0$. When the quadratic coefficient vanishes, the more general affine ansatz gives $h=px+(p^2-1)t+q$.

A narrower ansatz $h=a t^{-1/3}(1-x^2/t^{2/3})-bt$ fixes two coefficients together and permits exactly $(a,b)=(1/6,3/4)$ or $(0,1)$. The zero value of $a$ is a valid spatially constant branch, not an algebraic exception to discard. These finite-parameter families are exact solutions; they are not the complete general solution of the nonlinear [partial differential equation](partial-differential-equation-split.md), and their sums need not be solutions.

## ↑ Ancestors (7)

1. [Nonlinear diffusion equation](nonlinear-diffusion-equation.md)
2. [Diffusion equation](diffusion-equation-split.md)
3. [Partial differential equation](partial-differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
