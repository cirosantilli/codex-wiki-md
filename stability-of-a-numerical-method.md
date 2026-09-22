# Stability of a numerical method

↑ **Parent:** [Numerical analysis](numerical-analysis-split.md)

For a numerical evolution, [numerical stability](stability-of-a-numerical-method.md) means that perturbations remain controlled over a fixed finite interval by a bound independent of sufficiently small discretization parameters. With perturbations $\delta_n$ to starting data and added step defects $d_n$, a typical estimate is

$$
\max_{nh\leq T}\|\delta_n\|\leq C_T\left(\|\delta_0\|+\sum_{nh<T}\|d_n\|\right),
$$

where $C_T$ is independent of $h$. For a linear homogeneous recurrence, a uniform bound on powers of its update [matrix](matrix.md) supplies this control. [von Neumann stability analysis](von-neumann-stability-analysis.md) and the [energy method](energy-method.md) provide complementary tools.

Finite-interval [numerical stability](stability-of-a-numerical-method.md) differs from [absolute stability](linear-stability-domain.md) at a fixed step size. Applying the [Euler method](euler-method.md) to $y'=-2y$ multiplies a perturbation by $1-2h$ each step. At $h=0.2$ this is $0.6$, so perturbations shrink; at $h=1.2$ it is $-1.4$, so they alternate and grow. Nevertheless the [Euler method](euler-method.md) converges as $h\to0$ for this problem: failure at a coarse step does not contradict the convergence theorem. [Absolute stability](linear-stability-domain.md) asks whether a selected step preserves boundedness of the [Dahlquist test equation](dahlquist-test-equation.md) over arbitrarily many steps. MIT's analysis uses strict decay, $|1+h\lambda|<1$, rather than the boundary-inclusive boundedness convention.[Laurent Demanet, MIT 18.330, Chapter 5, Example 14, 2012](https://ocw.mit.edu/courses/18-330-introduction-to-numerical-analysis-spring-2012/a9d2bd9be098f0ada172af40379a17cc_MIT18_330S12_Chapter5.pdf)

## ↑ Ancestors (5)

1. [Numerical analysis](numerical-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (23)

- [Discrete L2 norm](discrete-l2-norm.md)
- [Global discretization error](global-discretization-error.md)
- [Implicit time-stepping method](implicit-time-stepping-method.md)
- [Order of a numerical method](order-of-a-numerical-method.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-57/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-60/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-69/3/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/1/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-63/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/5/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
