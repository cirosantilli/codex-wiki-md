# Stability of a two-parameter implicit-explicit diffusion scheme

↑ **Parent:** [von Neumann stability analysis](von-neumann-stability-analysis.md)

For the scheme

$$
\left(aI-\frac{\mu-c}{4}L\right)u^{n+1}
=\left(aI+\frac{\mu+c}{4}L\right)u^n,
$$

where $L=[1,-2,1]$ is the Dirichlet second-difference matrix and $\mu>0$, the modal amplification factor is

$$
G(s)=\frac{a-(\mu+c)s}{a+(\mu-c)s},
\qquad 0<s<1.
$$

Mesh-uniform stability holds exactly when

$$
a\geq0,
\qquad
c\leq a.
$$

For consistency with $u_t=u_{xx}$ under the displayed normalization one additionally chooses $a=1/2$; stability then requires $c\leq1/2$.

## ↑ Ancestors (8)

1. [von Neumann stability analysis](von-neumann-stability-analysis.md)
2. [Finite difference method](finite-difference-method.md)
3. [Finite difference](finite-difference-split.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ii/paper-3/40c/b/solution.md)
