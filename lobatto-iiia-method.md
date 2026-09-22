# Lobatto IIIA method

↑ **Parent:** [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)

A Lobatto IIIA method collocates at the [Lobatto quadrature](lobatto-quadrature.md) nodes, including both endpoints of the time interval. Its three-stage version has

$$
A=\begin{pmatrix}0&0&0\\5/24&1/3&-1/24\\1/6&2/3&1/6\end{pmatrix},
\qquad b=(1/6,2/3,1/6)^T,
\qquad c=(0,1/2,1)^T.
$$

The [Butcher order conditions](butcher-order-condition.md) give order four. Its [stability function](stability-function.md) is

$$
R(z)=\frac{1+z/2+z^2/12}{1-z/2+z^2/12},
$$

which is [A-stable](a-stability.md) but not [L-stable](l-stability.md). It is not [algebraically stable](algebraic-stability-of-a-runge-kutta-method.md): the first diagonal entry of the defining [matrix](matrix.md) is $2b_1a_{11}-b_1^2=-1/36$. This distinguishes linear [A-stability](a-stability.md) from nonlinear [algebraic stability](algebraic-stability-of-a-runge-kutta-method.md).

## ↑ Ancestors (8)

1. [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)
2. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
3. [Runge-Kutta method](runge-kutta-method.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (14)

- [Lobatto quadrature](lobatto-quadrature.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-69/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-71/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-63/4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/2/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/2/c/solution.md)
