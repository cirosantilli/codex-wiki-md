# Two-dimensional leapfrog stability threshold

↑ **Parent:** [Leapfrog advection scheme](leapfrog-advection-scheme.md)

For $u_t=u_x+u_y$ with equal spatial mesh sizes, the centered leapfrog recurrence has [amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md) $G^2-2i\mu(\sin\xi+\sin\eta)G-1$. Uniform [stability](stability-of-a-numerical-method.md) for arbitrary two-level starting perturbations holds exactly for $0<\mu<1/2$. At $\mu=1/2$ the phase pair $(\pi/2,\pi/2)$ gives $(G-i)^2$, and its [companion matrix](companion-matrix.md) has a nontrivial [Jordan block](jordan-block.md), producing growth proportional to the number of steps. For larger $\mu$ one [polynomial root](root-of-a-polynomial.md) has modulus greater than one. Bounds on [eigenvalue](eigenvalue.md) moduli alone therefore give a misleading non-strict endpoint.

## ↑ Ancestors (10)

1. [Leapfrog advection scheme](leapfrog-advection-scheme.md)
2. [Amplification polynomial of a multilevel finite difference scheme](amplification-polynomial-of-a-multilevel-finite-difference-scheme.md)
3. [von Neumann stability analysis](von-neumann-stability-analysis.md)
4. [Finite difference method](finite-difference-method.md)
5. [Finite difference](finite-difference-split.md)
6. [Numerical analysis](numerical-analysis-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-67/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/2/b/solution.md)
