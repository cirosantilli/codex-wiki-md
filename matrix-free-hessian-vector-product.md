# Matrix-free Hessian-vector product

↑ **Parent:** [Hessian matrix](hessian-matrix.md)

Applying a [Hessian matrix](hessian-matrix.md) to a [vector](vector.md) without explicitly storing all its entries. For $H=A^{\mathsf T}\Delta A$ with diagonal $\Delta$, evaluate $Hv=A^{\mathsf T}(\Delta(Av))$. This uses two matrix-vector multiplications and a diagonal scaling: $O(nd)$ arithmetic for dense $A\in\mathbb R^{n\times d}$, rather than forming the $d\times d$ [Hessian matrix](hessian-matrix.md). Iterative second-order methods can use this operation, with safeguards for indefinite curvature when the objective is nonconvex.

## ↑ Ancestors (8)

1. [Hessian matrix](hessian-matrix.md)
2. [Multivariable calculus](multivariable-calculus-split.md)
3. [Calculus](calculus-split.md)
4. [Real analysis](real-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Hessian of a sum of functions of linear forms](hessian-of-a-sum-of-functions-of-linear-forms.md)
- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2019/discrete-mathematics-continuous-mathematics-and-probability/6/c/iv/solution.md)
