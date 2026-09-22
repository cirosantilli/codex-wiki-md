# Lasso support bound from sparse eigenvalues

↑ **Parent:** [Sparse maximum eigenvalue](sparse-maximum-eigenvalue.md)

For $\lambda>0$ and $\phi>0$, use the [Lasso](lasso.md) objective $\|Y-X\beta\|_2^2/(2n)+\lambda\|\beta\|_1$. Suppose the noise score has maximum [norm](norm.md) at most $\lambda/2$, the true support has size $s$, and $\|X(\widehat\beta-\beta^0)\|_2^2/n\le16\lambda^2s/\phi^2$. For any nonempty $B\subseteq\widehat S$, the [Karush-Kuhn-Tucker conditions](karush-kuhn-tucker-conditions.md) imply

$$
\lambda|B|/2\le n^{-1}\operatorname{sgn}(\widehat\beta_B)^TX_B^TX(\beta^0-\widehat\beta)\le4\lambda\kappa_{|B|}\sqrt{|B|s}/\phi.
$$

The upper bound is the [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Hence $|B|\le64\kappa_{|B|}^2s/\phi^2$. A finite first index $m_*$ violating this inequality must exceed $|\widehat S|$. Its minimality also gives $|\widehat S|\le64\kappa_{m_*}^2s/\phi^2$. If no such index exists within $1,\ldots,p$, use the always defined bound $|\widehat S|\le64\kappa_p^2s/\phi^2$.

## ↑ Ancestors (6)

1. [Sparse maximum eigenvalue](sparse-maximum-eigenvalue.md)
2. [Lasso](lasso.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)
