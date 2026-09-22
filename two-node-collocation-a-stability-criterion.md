# Two-node collocation A-stability criterion

↑ **Parent:** [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)

For distinct nodes $c_1,c_2\in[0,1]$, the two-stage [collocation Runge-Kutta method](collocation-runge-kutta-method.md) has [stability function](stability-function.md)

$$
R(z)=\frac{1+(1-a)z+rz^2}{1-az+dz^2},\qquad a=(c_1+c_2)/2,\quad d=c_1c_2/2,\quad r=(1-c_1)(1-c_2)/2.
$$

The denominator has no zeros in the closed left half-plane. On the imaginary axis the denominator's squared modulus minus the numerator's is $(d^2-r^2)y^4$. Thus $d\geq r$, equivalently $c_1+c_2\geq1$, is necessary and sufficient for [A-stability](a-stability.md), using the [maximum modulus principle](maximum-modulus-principle.md) and the bound at infinity.

## ↑ Ancestors (8)

1. [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/3/b/solution.md)
