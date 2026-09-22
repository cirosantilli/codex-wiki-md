# Energy conservation for semidiscrete Galerkin advection

↑ **Parent:** [Finite element method](finite-element-method.md)

For periodic $u_t=u_x$, the conforming [Galerkin method](galerkin-method.md) has $M\dot U=CU$, with [mass matrix](mass-matrix.md) $M_{ij}=\int\phi_i\phi_j$ and $C_{ij}=\int\phi_i\phi_j'$. [Integration by parts](integration-by-parts.md) and periodicity give $C^T=-C$. Therefore

$$
\frac{d}{dt}(U^TMU)=2U^TCU=0.
$$

The conserved quantity is the squared [L2 norm](l2-norm.md) of the [finite element](finite-element.md) function. On a uniform one-dimensional mesh of spacing $h$, the [piecewise-linear hat functions](piecewise-linear-hat-function.md) give $M_{ii}=2h/3$, $M_{i,i\pm1}=h/6$, $C_{i,i+1}=1/2$ and $C_{i,i-1}=-1/2$.

## ↑ Ancestors (6)

1. [Finite element method](finite-element-method.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-341/5/b/solution.md)
