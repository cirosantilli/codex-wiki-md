# Newton correction compatibility condition

↑ **Parent:** [Multivariable Newton iteration](multivariable-newton-iteration.md)

A [multivariable Newton iteration](multivariable-newton-iteration.md) correction must solve the [linear system](system-of-linear-equations.md) $D\mathbf f(\mathbf x)\mathbf s=-\mathbf f(\mathbf x)$. It exists exactly when the right-hand side is in the image of the [Jacobian matrix](jacobian-matrix.md), and is unique when that [Jacobian matrix](jacobian-matrix.md) is invertible. At a [singular matrix](singular-matrix.md), there may be either no corrections or several; singularity alone does not decide which. For finding a [critical point](critical-point.md) of a scalar function $F$, use $\mathbf f=\nabla F$, so the [Jacobian matrix](jacobian-matrix.md) is the [Hessian matrix](hessian-matrix.md). Equal rows of the [Hessian matrix](hessian-matrix.md) with unequal corresponding [gradient](gradient.md) entries immediately make the correction [equations](equation.md) inconsistent.

## ↑ Ancestors (8)

1. [Multivariable Newton iteration](multivariable-newton-iteration.md)
2. [Newton iteration in a Banach space](newton-iteration-in-a-banach-space.md)
3. [Newton root-finding iteration](newton-root-finding-iteration.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-oxford/2021/prelims/mathematics-iv/7/b/solution.md)
