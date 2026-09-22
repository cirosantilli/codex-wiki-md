# Optimal rectangle bound for a quartic separable initial-value problem

↑ **Parent:** [Picard-Lindelöf theorem](picard-lindelof-theorem.md)

For the [ordinary differential equation](ordinary-differential-equation.md) $y'=3x^2/(4y^3)$ through $y(0)=b>0$, consider a symmetric existence rectangle $|x|\le h$, $|y-b|\le k<b$. Its maximum slope bound is $M=3h^2/[4(b-k)^3]$. The condition $Mh\le k$ becomes $h^3\le4k(b-k)^3/3$. Differentiating $k(b-k)^3$ shows its maximum occurs at $k=b/4$, giving

$$
h\le\frac{3^{2/3}b^{4/3}}4.
$$

This is the largest interval guaranteed by this particular centered-rectangle criterion. Direct [separation of variables](separation-of-variables.md) instead gives $y(x)=(b^4+x^3)^{1/4}$ on the maximal real interval $x>-b^{4/3}$. The comparison shows the difference between a sufficient local [existence theorem](picard-lindelof-theorem.md) and the actual continuation interval. The endpoint obstruction is the zero of the denominator at $y=0$.

## ↑ Ancestors (7)

1. [Picard-Lindelöf theorem](picard-lindelof-theorem.md)
2. [Ordinary differential equation](ordinary-differential-equation.md)
3. [Differential equation](differential-equation-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)
