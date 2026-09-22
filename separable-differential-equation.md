# Separable differential equation

↑ **Parent:** [Ordinary differential equation](ordinary-differential-equation.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Separable_differential_equation)

A first-order [ordinary differential equation](ordinary-differential-equation.md) is separable if its explicit form factors as $y'=a(t)b(y)$. On an [interval](interval-mathematics.md) where $b(y)\ne0$, write $dy/b(y)=a(t)\,dt$ and take [antiderivatives](antiderivative.md) to obtain an [implicit solution](implicit-solution.md):

$$
\int\frac{dy}{b(y)}=\int a(t)\,dt+C.
$$

An [initial condition](initial-condition.md) determines $C$ and selects a branch and domain. The useful simplification is that the two [integrals](integral.md) each involve only one variable, even when the original equation is nonlinear.

For [Newton's law of cooling](newton-s-law-of-cooling.md), division by $y-T_a$ gives $dy/(y-T_a)=-k\,dt$. To keep the [logarithm](logarithm.md) dimensionless, integrate relative to the initial excess [temperature](temperature.md):

$$
\log\left|\frac{y(t)-T_a}{y_0-T_a}\right|=-k(t-t_0).
$$

When $y_0\ne T_a$, [continuity](continuous-function.md) preserves the sign of the excess [temperature](temperature.md) until any potential zero, giving $y-T_a=(y_0-T_a)e^{-k(t-t_0)}$. This formula never reaches zero at finite time. Taking its [derivative](derivative.md) verifies the [ordinary differential equation](ordinary-differential-equation.md), and substitution at $t_0$ verifies the [initial condition](initial-condition.md).

Always check what division removed. Each zero $b(y_*)=0$ gives a constant [solution of a differential equation](solution-of-a-differential-equation.md) $y=y_*$. Cooling therefore also has the [equilibrium point](equilibrium-point-of-a-dynamical-system.md) $y=T_a$, omitted by division but included in the final explicit formula. For the nonunique [initial value problem](initial-value-problem.md) $y'=\sqrt{|y|}$, division by $\sqrt{|y|}$ only describes the moving pieces: a valid solution may remain zero for an arbitrary time before joining one. Separation is a method for finding solutions, not a uniqueness theorem.

**Table of contents**

- [Cubic logistic differential equation](cubic-logistic-differential-equation.md)

## ↑ Ancestors (6)

1. [Ordinary differential equation](ordinary-differential-equation.md)
2. [Differential equation](differential-equation-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Newton's law of cooling](newton-s-law-of-cooling.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ia/paper-2/2d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/ia/paper-2/7b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ia/paper-2/5a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-68/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/ia/paper-2/2b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-1/31e/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-310/1/a/solution.md)
