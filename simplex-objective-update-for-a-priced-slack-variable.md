# Simplex objective update for a priced slack variable

↑ **Parent:** [Simplex tableau](simplex-tableau.md)

If a variable $x_k$ gains an objective coefficient $p$, the new objective is $z=z_{\rm old}+px_k$. Substitute this in the old canonical objective equation and eliminate any remaining basic-column coefficients using the constraint rows. If $x_k$ is nonbasic, this simply subtracts $p$ from its objective-row coefficient. When a [slack variable](slack-variable.md) is sold, rename the old slack as the sales quantity; its equation already gives the correct equality and no new slack is added. Reoptimization can then start directly from the altered [simplex tableau](simplex-tableau.md).

## ↑ Ancestors (7)

1. [Simplex tableau](simplex-tableau.md)
2. [Simplex method](simplex-method.md)
3. [Linear programming](linear-programming.md)
4. [Mathematical optimization](mathematical-optimization-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-35/2/c/solution.md)
