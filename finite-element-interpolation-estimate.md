# Finite element interpolation estimate

↑ **Parent:** [Finite element method](finite-element-method.md)

On a [shape-regular mesh](shape-regular-mesh.md) in dimensions at most three, nodal piecewise-linear interpolation of $u\in H^2(\Omega)$ satisfies

$$
\|u-I_hu\|_{L^2(\Omega)}+h\|u-I_hu\|_{H^1(\Omega)}
\leq Ch^2\|u\|_{H^2(\Omega)},
$$

where $h$ is the largest element diameter and $C$ is independent of $h$. For homogeneous [Dirichlet boundary conditions](dirichlet-boundary-condition.md), $I_hu$ belongs to the [conforming finite element space](conforming-finite-element-space.md). Scaling each element to a reference element gives the estimate; [shape regularity](shape-regular-mesh.md) bounds the scaling constants, while subtraction of an [affine function](affine-function.md) leaves an error controlled by the second derivatives.

## ↑ Ancestors (6)

1. [Finite element method](finite-element-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Aubin–Nitsche duality argument](aubin-nitsche-duality-argument.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/7/solution.md)
- [Shape-regular mesh](shape-regular-mesh.md)
