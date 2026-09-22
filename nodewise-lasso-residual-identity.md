# Nodewise-Lasso residual identity

↑ **Parent:** [Nodewise Lasso](nodewise-lasso.md)

For [Nodewise Lasso](nodewise-lasso.md) with objective $\|X_j-X_{-j}\gamma\|_2^2/(2n)+\lambda_j\|\gamma\|_1$, put $r_j=X_j-X_{-j}\widehat\gamma^{(j)}$. Its [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) give $X_{-j}^Tr_j/n=\lambda_jz_j$ with $z_j\in\partial\|\widehat\gamma^{(j)}\|_1$. Hence

$$
X_j^Tr_j/n=\|r_j\|_2^2/n+\lambda_j\|\widehat\gamma^{(j)}\|_1=\widehat\tau_j^2.
$$

For $\lambda_j>0$ this is positive whenever $X_j\ne0$; if it were zero both nonnegative terms would vanish, forcing $\widehat\gamma^{(j)}=0$ and $X_j=r_j=0$. Nonzero columns are therefore an essential hypothesis for division by this quantity.

## ↑ Ancestors (7)

1. [Nodewise Lasso](nodewise-lasso.md)
2. [Debiased Lasso](debiased-lasso.md)
3. [Lasso](lasso.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Debiased-Lasso remainder bound](debiased-lasso-remainder-bound.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-205/6/solution.md)
