# Semistrip Dirichlet-to-Neumann sine transforms

↑ **Parent:** [Dirichlet-to-Neumann map](dirichlet-to-neumann-map.md)

In the [semistrip Laplace spectral global relation](semistrip-laplace-spectral-global-relation.md), reality makes $W(\pm\kappa)$ real for $\kappa>0$. Its imaginary parts at those two arguments remove the unknown vertical-side [normal derivative](normal-derivative.md). With $G_j^s(\kappa)=\int_0^\infty\sin(\kappa x)g_j(x)\,dx$ and $S_j(\kappa)=\int_0^\infty\sin(\kappa x)q_y(x,j)\,dx$, the result is

$$
S_0=\frac{\kappa[-\cosh(\kappa l)G_0^s+G_l^s+\int_0^l\sinh(\kappa(l-y))h(y)\,dy]}{\sinh(\kappa l)},\qquad
S_l=\frac{\kappa[-G_0^s+\cosh(\kappa l)G_l^s-\int_0^l\sinh(\kappa y)h(y)\,dy]}{\sinh(\kappa l)}.
$$

The lower outward [normal derivative](normal-derivative.md) is $-q_y$, so its [Dirichlet-to-Neumann map](dirichlet-to-neumann-map.md) coefficient is $-S_0$, whereas the upper coefficient is $S_l$.

// Target: analysis.bigb

## ↑ Ancestors (8)

1. [Dirichlet-to-Neumann map](dirichlet-to-neumann-map.md)
2. [Boundary value problem](boundary-value-problem.md)
3. [Ordinary differential equation](ordinary-differential-equation.md)
4. [Differential equation](differential-equation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-86/2/b/solution.md)
