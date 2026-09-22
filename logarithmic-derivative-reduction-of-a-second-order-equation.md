# Logarithmic-derivative reduction of a second-order equation

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)

Where $y\ne0$, its [logarithmic derivative](logarithmic-derivative.md) $q=y'/y$ changes this nonlinear second-order [ordinary differential equation](ordinary-differential-equation.md) into the [first-order linear differential equation](first-order-linear-differential-equation.md) $q'=a(x)q$. For continuous $a$, initial values $y(x_0)=y_0\ne0$ and $y'(x_0)=v_0$ therefore give

$$
q(x)=\frac{v_0}{y_0}\exp\left(\int_{x_0}^x a(t)\,dt\right),\qquad
y(x)=y_0\exp\left(\int_{x_0}^x q(t)\,dt\right).
$$

Differentiation proves both the equation and the initial data. The exponential preserves the sign of $y_0$, so the solution never reaches the singular value zero on any finite interval where $a$ is continuous. For $a(x)=2x$ and $y_0=v_0=1$, the expression reduces to $y(x)=\exp(\int_0^x e^{t^2}\,dt)$.

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-algebra-1-and-differential-equations-1-course-of-the-university-of-oxford/2015/6/b/solution.md)
