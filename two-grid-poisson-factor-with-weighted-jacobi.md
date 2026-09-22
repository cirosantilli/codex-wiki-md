# Two-grid Poisson factor with weighted Jacobi

↑ **Parent:** [Multigrid method](multigrid-method.md)

For the one-dimensional [Poisson equation](poisson-equation.md), use linear interpolation, [full-weighting restriction](full-weighting-restriction.md), an exact coarse solve, and one pre- and one post-sweep of [weighted Jacobi](weighted-jacobi-method.md) with weight $2/3$. On a pair of harmonics $\theta,\theta+\pi$, put $s=\sin^2(\theta/2)$ and $c=1-s$. The coarse correction is $C=\left(\begin{smallmatrix}s&-c\\-s&c\end{smallmatrix}\right)$, and the smoother is $S=\operatorname{diag}(1-4s/3,1-4c/3)$. The rank-one error operator $SCS$ has nonzero eigenvalue $s(1-4s/3)^2+c(1-4c/3)^2=1/9$. This exact harmonic calculation illustrates mesh-independent two-grid contraction for the constant-coefficient model; it is not an unconditional result for arbitrary operators or transfer choices.

## ↑ Ancestors (6)

1. [Multigrid method](multigrid-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/7/solution.md)
