# Interior absolute-error rate of the Nadaraya-Watson estimator

↑ **Parent:** [Nadaraya–Watson estimator](nadaraya-watson-estimator.md)

For the unit-width symmetric box [kernel for density estimation](kernel-for-density-estimation.md), suppose the design density is positive and differentiable at $x$, the regression function is twice differentiable there, and the conditional variance and design density are bounded near $x$. Write $G_n=(nh)^{-1}\sum_i(Y_i-m(x))\mathbf1_{\{|X_i-x|\le h/2\}}$. Symmetry cancels its linear Taylor term, giving $\mathbb EG_n=O(h^2)$; [independence](independent-random-variables.md) gives $\operatorname{Var}G_n=O((nh)^{-1})$. The [absolute error bound for a ratio estimator with a controlled denominator](absolute-error-bound-for-a-ratio-estimator-with-a-controlled-denominator.md) gives the displayed rate if the small-denominator contribution is negligible. The balance $h\asymp n^{-1/5}$ gives $O(n^{-2/5})$. Interior design positivity matters: support boundaries can prevent the linear cancellation.

## ↑ Ancestors (9)

1. [Nadaraya–Watson estimator](nadaraya-watson-estimator.md)
2. [Local polynomial regression](local-polynomial-regression.md)
3. [Nonparametric regression](nonparametric-regression.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/4/solution.md)
