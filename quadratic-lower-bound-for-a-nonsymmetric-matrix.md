# Quadratic lower bound for a nonsymmetric matrix

↑ **Parent:** [Invertible matrix](invertible-matrix.md)

Let $B$ be a real square [matrix](matrix.md) and suppose $x^TBx\geq c|x|^2$ for every real [vector](vector.md) $x$, with $c>0$. The [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) gives $x^TBx\leq|x|\,|Bx|$, hence $|Bx|\geq c|x|$ for all $x$. In particular the [kernel](kernel-of-a-linear-map-split.md) is zero, so $B$ is an [invertible matrix](invertible-matrix.md). Applying the bound to $x=B^{-1}y$ gives the [operator norm](operator-norm.md) estimate $\|B^{-1}\|\leq1/c$ in the [Euclidean norm](euclidean-norm.md).

Symmetry of $B$ is unnecessary: $x^TBx=x^THx$ for its [symmetric part of a matrix](symmetric-part-of-a-matrix.md) $H=(B+B^T)/2$. Thus the hypothesis is exactly a positive lower bound on that [symmetric matrix](symmetric-matrix.md), even when the antisymmetric part is nonzero.

## ↑ Ancestors (6)

1. [Invertible matrix](invertible-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
