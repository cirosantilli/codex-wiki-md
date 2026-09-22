# Norm of a two-endpoint interpolation projection

↑ **Parent:** [Projection (linear algebra)](projection-linear-algebra.md)

Let $\ell_0,\ell_1$ be norm-one extensions to $L^\infty((0,1))$ of endpoint [point evaluations](point-evaluation-functional.md) on $C([0,1])$. For [continuous functions](continuous-function.md) $e_0,e_1$ with $e_i(j)=\delta_{ij}$, the [linear projection](projection-linear-algebra.md) $Pf=\ell_0(f)e_0+\ell_1(f)e_1$ has the displayed [operator norm](operator-norm.md), independently of which extensions are chosen.

The [triangle inequality](triangle-inequality.md) proves the upper bound. At a point $x_*$ maximizing $|e_0|+|e_1|$, choose unit complex numbers $a_j$ with $a_je_j(x_*)=|e_j(x_*)|$. The [continuous function](continuous-function.md) $f(x)=(1-x)a_0+xa_1$ has [supremum norm](supremum-norm.md) one and $\ell_j(f)=a_j$, so $(Pf)(x_*)=|e_0(x_*)|+|e_1(x_*)|$. The [L-infinity norm](l-infinity-norm.md) of the continuous output equals its [supremum norm](supremum-norm.md), proving equality even at an endpoint.

## ↑ Ancestors (9)

1. [Projection (linear algebra)](projection-linear-algebra.md)
2. [Linear operator](linear-operator.md)
3. [Linear map](linear-map.md)
4. [Vector space](vector-space-split.md)
5. [Linear algebra](linear-algebra-split.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-functional-analysis-i-course-of-the-university-of-oxford/2023/3/c/ii/solution.md)
