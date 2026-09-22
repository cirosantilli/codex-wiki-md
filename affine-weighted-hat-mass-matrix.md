# Affine-weighted hat mass matrix

↑ **Parent:** [Mass matrix](mass-matrix.md)

On a one-dimensional uniform [finite element mesh](finite-element-mesh.md) of spacing $h$, let $w$ be an [affine function](affine-function.md) and $\phi_i$ the interior [piecewise-linear hat functions](piecewise-linear-hat-function.md). The weighted [mass matrix](mass-matrix.md) has entries

$$
W_{ii}=\frac{2h}{3}w(x_i),\qquad
W_{i,i+1}=W_{i+1,i}=\frac h{12}\bigl(w(x_i)+w(x_{i+1})\bigr),
$$

and zero entries for nonadjacent indices. The diagonal product $\phi_i^2$ is symmetric about $x_i$ and integrates to $2h/3$; the neighbouring product is symmetric about $(x_i+x_{i+1})/2$ and integrates to $h/6$. The odd part of an [affine function](affine-function.md) integrates to zero around each centre, giving the formulas. This evaluates a variable reaction term exactly without substituting a constant coefficient or a quadrature approximation.

## ↑ Ancestors (7)

1. [Mass matrix](mass-matrix.md)
2. [Finite element method](finite-element-method.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-72/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-341/5/iii/solution.md)
