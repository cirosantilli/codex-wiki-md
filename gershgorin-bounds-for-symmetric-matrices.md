# Gershgorin bounds for symmetric matrices

↑ **Parent:** [Gershgorin circle theorem](gershgorin-circle-theorem.md)

For a real [symmetric matrix](symmetric-matrix.md), or more generally a [Hermitian matrix](hermitian-operator.md), the [finite-dimensional spectral theorem](finite-dimensional-spectral-theorem.md) makes all [eigenvalues](eigenvalue.md) real. Intersecting its [Gershgorin discs](gershgorin-disc.md) with the real axis gives

$$
\lambda\in\bigcup_{i=1}^n[a_{ii}-r_i,a_{ii}+r_i],\qquad \min_i(a_{ii}-r_i)\leq\lambda\leq\max_i(a_{ii}+r_i).
$$

The union preserves gaps that the single outer [interval](interval-mathematics.md) loses. If every $a_{ii}-r_i>0$, all [eigenvalues](eigenvalue.md) are positive, so the [matrix](matrix.md) is a [positive-definite matrix](positive-definite-matrix.md). This is the positive-diagonal [strictly diagonally dominant matrix](strictly-diagonally-dominant-matrix.md) criterion. For the three-by-three example, $1.7\leq\lambda\leq9.4$ gives a [positive-definite matrix](positive-definite-matrix.md) certificate and bounds its [spectral condition number of a positive-definite matrix](spectral-condition-number-of-a-positive-definite-matrix.md) by $9.4/1.7\approx5.529412$; the computed value is about $4.544364$.

Strictness matters. The [symmetric matrix](symmetric-matrix.md) $\left(\begin{smallmatrix}1&-1\\-1&1\end{smallmatrix}\right)$ has positive diagonal and is a [diagonally dominant matrix](diagonally-dominant-matrix.md), but its [eigenvalues](eigenvalue.md) are $0$ and $2$: it is singular. For a general complex [matrix](matrix.md), the condition $\operatorname{Re}a_{ii}>r_i$ only puts the [eigenvalues](eigenvalue.md) in the open [right half-plane](right-half-plane.md). The [Hermitian matrix](hermitian-operator.md) assumption is what converts that statement into positive definiteness.

## ↑ Ancestors (6)

1. [Gershgorin circle theorem](gershgorin-circle-theorem.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Gershgorin circle theorem](gershgorin-circle-theorem.md)
- [Gershgorin stability bound for a variable-coefficient diffusion stencil](gershgorin-stability-bound-for-a-variable-coefficient-diffusion-stencil.md)
