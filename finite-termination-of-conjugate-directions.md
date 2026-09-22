# Finite termination of conjugate directions

↑ **Parent:** [Conjugate direction](conjugate-direction.md)

Let $p_1,\ldots,p_n$ be [conjugate directions](conjugate-direction.md) for a [symmetric positive-definite matrix](symmetric-positive-definite-matrix.md) $A$. Starting from any $x_1$, minimize $x^TAx/2-b^Tx$ successively along those full lines, stopping early if the [linear-system residual](linear-system-residual.md) $r_j=b-Ax_j$ vanishes. The [quadratic minimization along a line](quadratic-minimization-along-a-line.md) uses $\alpha_j=p_j^Tr_j/(p_j^TAp_j)$ and gives $r_{j+1}=r_j-\alpha_jAp_j$.

This makes $p_j^Tr_{j+1}=0$. For $i<j$, conjugacy preserves $p_i^Tr_{j+1}=p_i^Tr_j$. By [mathematical induction](mathematical-induction.md), $r_{j+1}$ is [orthogonal](orthogonal-vectors.md) to all preceding search [vectors](vector.md). The $n$ [conjugate directions](conjugate-direction.md) are [linearly independent](linear-independence.md) and hence form a [basis](basis.md), so $r_{n+1}=0$. Thus the method reaches the unique solution of the [linear system](system-of-linear-equations.md) in at most $n$ steps in exact arithmetic. The [conjugate gradient method](conjugate-gradient-method.md) generates such directions without storing a complete prescribed [basis](basis.md) in advance.

## ↑ Ancestors (8)

1. [Conjugate direction](conjugate-direction.md)
2. [Conjugate gradient method](conjugate-gradient-method.md)
3. [Gradient descent](gradient-descent-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2011/3/c/solution.md)
