# Finite element mesh

↑ **Parent:** [Finite element method](finite-element-method.md)

A [finite element mesh](finite-element-mesh.md) partitions a domain into simple regions called elements, such as [intervals](interval-mathematics.md), [triangles](triangle.md) or [tetrahedra](tetrahedron.md). In a conforming partition, distinct element interiors are disjoint, their closures cover the domain closure, and any nonempty intersection is a common face, edge or vertex of both elements. Chen's author notes give this compatibility condition for simplicial [meshes](finite-element-mesh.md).[Long Chen, Introduction to Finite Element Methods, §2.1, pp. 3–4; updated January 17, 2024](https://webapps.math.uci.edu/~chenlong/226/Ch2FEM.pdf) Local [piecewise polynomial functions](piecewise-polynomial-function.md) and local [integrals](integral.md) are defined on these regions; compatible degrees of freedom join them into a global [conforming finite element space](conforming-finite-element-space.md). The assembled [stiffness matrix](stiffness-matrix.md) and [mass matrix](mass-matrix.md) then inherit the local overlap pattern.

For the [finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md), a [mesh](finite-element-mesh.md) is simply an ordered list

$$
0=x_0<x_1<\cdots<x_n=1,\qquad
\mathcal T_h=\{[x_j,x_{j+1}]:0\leq j<n\},\qquad
h=\max_{0\leq j<n}(x_{j+1}-x_j).
$$

Nodes are the endpoints; elements are the intervening [intervals](interval-mathematics.md). Four equal elements have five nodes but only three unknown nodal values after imposing the zero [Dirichlet boundary conditions](dirichlet-boundary-condition.md). A nonuniform partition such as $0,1/8,1/4,1/2,1$ has element lengths $1/8,1/8,1/4,1/2$ and $h=1/2$, so counting elements alone does not measure the largest unresolved scale.

Refining a [finite element mesh](finite-element-mesh.md) replaces some or all elements by smaller ones. For continuous [piecewise linear functions](piecewise-linear-function.md) in one dimension, retaining all old nodes gives nested [conforming finite element spaces](conforming-finite-element-space.md) $V_h\subset V_{h/2}$ when every [interval](interval-mathematics.md) is bisected. The old approximation remains available, and the new interior nodes allow additional changes of slope. With a symmetric [coercive bilinear form](coercive-bilinear-form.md) and exact integration, best approximation from [Galerkin orthogonality](galerkin-orthogonality.md) means that the [energy norm](energy-norm.md) error cannot increase under such nested refinement.

For the [finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md), uniform refinement from four to eight elements increases the unknown count from three to seven. The exact formulas give maximum errors $0.0078125$ and $0.001953125$, and [energy norm](energy-norm.md) errors approximately $0.0721688$ and $0.0360844$. Refinement near a region of strong curvature can spend unknowns where the [linear interpolation](linear-interpolation.md) error matters most; convergence in a general problem still needs approximation and regularity assumptions such as those in the [finite element interpolation estimate](finite-element-interpolation-estimate.md).

**Table of contents**

- [Shape-regular mesh](shape-regular-mesh.md)

## ↑ Ancestors (6)

1. [Finite element method](finite-element-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (9)

- [Affine-weighted hat mass matrix](affine-weighted-hat-mass-matrix.md)
- [Finite element](finite-element.md)
- [Finite element mesh](finite-element-mesh.md)
- [Finite element method](finite-element-method.md)
- [Finite element solution of the one-dimensional Poisson equation](finite-element-solution-of-the-one-dimensional-poisson-equation.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-341/6/solution.md)
- [Piecewise-linear hat function](piecewise-linear-hat-function.md)
