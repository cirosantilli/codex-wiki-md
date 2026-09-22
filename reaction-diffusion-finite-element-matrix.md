# Reaction-diffusion finite element matrix

↑ **Parent:** [Stiffness matrix](stiffness-matrix.md)

For $-u''+u=f$ with homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md), the conforming [piecewise-linear hat functions](piecewise-linear-hat-function.md) on a uniform grid give a diffusion [stiffness matrix](stiffness-matrix.md) $S$ and a [mass matrix](mass-matrix.md) $M$. Their nonzero entries are $S_{ii}=2/h$, $S_{i,i+1}=-1/h$, $M_{ii}=2h/3$, and $M_{i,i+1}=h/6$, with symmetric counterparts. The sum is a [positive-definite matrix](positive-definite-matrix.md) because its coefficient [quadratic form](quadratic-form.md) is $\int((u_h')^2+u_h^2)$. For forcing $f(x)=x$, the load at $x_i$ is $hx_i$.

## ↑ Ancestors (7)

1. [Stiffness matrix](stiffness-matrix.md)
2. [Finite element method](finite-element-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/5/c/solution.md)
