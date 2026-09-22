# Fourth-order conditions for a Runge-Kutta method

↑ **Parent:** [Butcher order condition](butcher-order-condition.md)

With $c=Ae$ and $C=\operatorname{diag}(c)$, a [Runge-Kutta method](runge-kutta-method.md) has order at least four exactly when the eight [Butcher order conditions](butcher-order-condition.md)

$$
b^Te=1,\quad b^Tc=\frac12,\quad b^Tc^2=\frac13,\quad b^TAc=\frac16,\quad b^Tc^3=\frac14,\quad b^TCAc=\frac18,\quad b^TAc^2=\frac1{12},\quad b^TA^2c=\frac1{24}
$$

hold; powers of $c$ are componentwise. These conditions match the numerical and exact coefficients indexed by [rooted trees](rooted-tree.md) through order four. Matching the scalar [Dahlquist test equation](dahlquist-test-equation.md) alone is insufficient to check the nonlinear [Butcher order conditions](butcher-order-condition.md).

## ↑ Ancestors (7)

1. [Butcher order condition](butcher-order-condition.md)
2. [Runge-Kutta method](runge-kutta-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Classical fourth-order Runge-Kutta method](classical-fourth-order-runge-kutta-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/2/a/solution.md)
