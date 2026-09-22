# Energy stability for variable-coefficient reaction diffusion

↑ **Parent:** [Energy method](energy-method.md)

For a zero-boundary centered semidiscretization $U'=D_hU+V_hU$, where $D_h$ is the scaled [Dirichlet discrete Laplacian](dirichlet-discrete-laplacian.md) and $V_h=\operatorname{diag}(a_j)$ with $a_j\leq a_+$, [summation by parts](abel-s-summation-formula.md) gives $(U,D_hU)_h\leq0$. Hence $\tfrac12(d/dt)\|U\|_h^2\leq a_+\|U\|_h^2$. The [Gronwall inequality](gronwall-inequality.md) yields $\|U(t)\|_h\leq e^{a_+t}\|U(0)\|_h$, a mesh-independent [stability](stability-of-a-numerical-method.md) bound on every fixed finite interval. Positive reaction coefficients can permit physical growth without violating this form of [stability](stability-of-a-numerical-method.md).

## ↑ Ancestors (6)

1. [Energy method](energy-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-68/5/a/solution.md)
