<h1 id="5j/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

At a current value $\beta$, put

$$
\eta_i=x_i^T\beta=g(\mu_i),
\qquad
W_{ii}=
\frac1{a_i\sigma^2V(\mu_i)\{g'(\mu_i)\}^2},
$$

and define the working response

$$
z_i=\eta_i+(Y_i-\mu_i)g'(\mu_i).
$$

Then the displayed formulas in the question can be written compactly as

$$
\mathcal I(\beta)=X^TWX,
$$

and

$$
U(\beta)=X^TW(z-X\beta).
$$

Indeed, the $j$th component of the latter is

$$
\sum_{i=1}^n
\frac{X_{ij}(Y_i-\mu_i)}
{a_i\sigma^2V(\mu_i)g'(\mu_i)},
$$

which is precisely the stated score.

Substitution into the Fisher-scoring update gives

$$
\beta^{\rm new}
=\beta+(X^TWX)^{-1}X^TW(z-X\beta)
=(X^TWX)^{-1}X^TWz.
$$

By part (b), this is the [weighted least squares](../../../../../../weighted-least-squares.md) fit of the working response $z$ on $X$. Both $z$ and $W$ are recomputed from the current fitted means after every update. Fisher scoring for a [generalized linear model](../../../../../../generalized-linear-model.md) is therefore the [iteratively reweighted least squares](../../../../../../iteratively-reweighted-least-squares.md) algorithm.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [5J](../../5j.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
