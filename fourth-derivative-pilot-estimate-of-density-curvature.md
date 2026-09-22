# Fourth-derivative pilot estimate of density curvature

↑ **Parent:** [Plug-in bandwidth selection](plug-in-bandwidth-selection.md)

Twice integrating by parts gives $R(f'')=\int f f^{(4)}$. Estimate this by averaging a fourth-derivative [kernel density estimator](kernel-density-estimation.md) at the observations. Its expectation contains diagonal term $K^{(4)}(0)/(ng^5)$ and leading smoothing bias $-g^2\mu_2(K)R(f''')/2$. Balancing them yields pilot scale $g\asymp R(f''')^{-1/7}n^{-1/7}$. With suitable derivatives and tails, the estimation error is bounded by $O_p(g^2+(ng^5)^{-1}+n^{-1/2}+n^{-1}g^{-9/2})$, giving an $O_p(n^{-2/7})$ relative-bandwidth bound after substitution. More carefully calibrated bias cancellation can improve that bound.

// Target: statistical-inference.bigb

## ↑ Ancestors (11)

1. [Plug-in bandwidth selection](plug-in-bandwidth-selection.md)
2. [Smoothing bandwidth](smoothing-bandwidth.md)
3. [Kernel for nonparametric regression](kernel-for-nonparametric-regression.md)
4. [Local polynomial regression](local-polynomial-regression.md)
5. [Nonparametric regression](nonparametric-regression.md)
6. [Nonparametric statistics](nonparametric-statistics-split.md)
7. [Statistical inference](statistical-inference-split.md)
8. [Probability and statistics](probability-and-statistics-split.md)
9. [Area of mathematics](area-of-mathematics.md)
10. [Mathematics](mathematics-split.md)
11. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-42/4/solution.md)
