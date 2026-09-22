# Slope parameter for a homogeneous first-order equation

↑ **Parent:** [Homogeneous first-order differential equation](homogeneous-first-order-differential-equation.md)

An implicit [homogeneous first-order differential equation](homogeneous-first-order-differential-equation.md) $y/x=F(p)$, where $p=dy/dx$, can be reduced by treating the slope as an auxiliary variable. Differentiating $y=xF(p)$ gives

$$
p=F(p)+xF'(p)\frac{dp}{dx},\qquad
\frac{dx}{x}=\frac{F'(p)}{p-F(p)}\,dp.
$$

Where the divisions are valid, this is a [separable differential equation](separable-differential-equation.md). Constant slopes lost when dividing by $p-F(p)$ must be checked in the original equation.

For $F(p)=2p/(1-p^2)$, the reduced equation is $2xp'=-p(1-p^2)$ and its nonconstant solutions obey $xp^2/(1-p^2)=C$. Substitution recovers the [parabolas](parabola.md) $y^2=4C(x+C)$, together with the constant solution $y=0$. Real graph branches must have $p^2=C/(x+C)\geq0$, and the original restrictions $x\ne0$, $p\ne\pm1$ still apply. The constant slopes $p=\pm1$ solve the reduced equation but are excluded from the original equation.

## ↑ Ancestors (7)

1. [Homogeneous first-order differential equation](homogeneous-first-order-differential-equation.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2016/paper-2/14/c/i/solution.md)
