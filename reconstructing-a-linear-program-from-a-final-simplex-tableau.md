# Reconstructing a linear program from a final simplex tableau

↑ **Parent:** [Simplex tableau](simplex-tableau.md)

For a maximization problem with unpriced unit [slack variables](slack-variable.md), their columns in a final [simplex tableau](simplex-tableau.md) give $B^{-1}$, where $B$ consists of the original basic columns. The constraint right side is $\bar b=B^{-1}b$, so $b=B\bar b$. If the objective row uses [reduced costs](reduced-cost.md) $r_j=c_j-c_B^TB^{-1}A_j$, its slack entries are $-y^T$ with $y^T=c_B^TB^{-1}$. Therefore $c_B^T=y^TB$. In a homogeneous linear objective with no constant offset, the displayed basic objective value must equal $c_B^T\bar b=y^Tb$. This identity detects inconsistent tableau constants; an affine offset affects the value but not the reduced costs.

## ↑ Ancestors (7)

1. [Simplex tableau](simplex-tableau.md)
2. [Simplex method](simplex-method.md)
3. [Linear programming](linear-programming.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-33/1/solution.md)
