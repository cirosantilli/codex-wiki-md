# Runge-Kutta contractivity identity

↑ **Parent:** [Algebraic stability of a Runge-Kutta method](algebraic-stability-of-a-runge-kutta-method.md)

For differences $D_i$ between corresponding stages and differences $F_i$ between their vector fields, a Runge--Kutta step satisfies

$$
\|d_{n+1}\|^2=\|d_n\|^2+2h\sum_i b_i\operatorname{Re}\langle D_i,F_i\rangle-h^2\sum_{i,j}m_{ij}\operatorname{Re}\langle F_i,F_j\rangle.
$$

To derive the identity, expand the squared [norm](norm.md) of $d_{n+1}=d_n+h\sum_i b_iF_i$ and substitute $d_n=D_i-h\sum_j a_{ij}F_j$ in the linear term. Symmetrizing the double sum gives the displayed coefficients $m_{ij}$. For a [dissipative vector field](dissipative-vector-field.md), the first sum is nonpositive when $b_i\geq0$, and the second sum is nonnegative when the [matrix](matrix.md) $(m_{ij})$ is a [positive semidefinite matrix](positive-semidefinite-matrix.md). Thus [algebraic stability](algebraic-stability-of-a-runge-kutta-method.md) implies [B-stability](b-stability.md).

## ↑ Ancestors (9)

1. [Algebraic stability of a Runge-Kutta method](algebraic-stability-of-a-runge-kutta-method.md)
2. [Collocation Runge-Kutta method](collocation-runge-kutta-method.md)
3. [Implicit Runge-Kutta method](implicit-runge-kutta-method.md)
4. [Runge-Kutta method](runge-kutta-method.md)
5. [Numerical analysis](numerical-analysis-split.md)
6. [Analysis](analysis-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Butcher contractivity theorem](butcher-contractivity-theorem.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-80/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/2/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/4/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/2/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-341/section-b/6/solution.md)
