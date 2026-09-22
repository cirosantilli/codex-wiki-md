<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For a spatially uniform [steady state](../../../../steady-state.md) with nonzero [bacteria](../../../../bacteria.md) abundance, $b(1-b)=0$ forces $b_*=1$. The [nutrient](../../../../nutrient.md) balance then gives

$$
\boxed{(b_*,n_*)=\left(1,\frac{\lambda}{\mu(1+b_0^2)}\right).}
$$

To test spatially uniform [linear stability](../../../../linear-stability.md), write

$$
F(b,n)=b(1-b),\qquad G(b,n)=\frac{\lambda b^2}{b_0^2+b^2}-\mu bn.
$$

At the positive [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md), the [Jacobian matrix](../../../../jacobian-matrix.md) is

$$
J_0=\begin{pmatrix}-1&0\\\eta&-\mu\end{pmatrix},\qquad
\eta=\frac{2\lambda b_0^2}{(1+b_0^2)^2}-\mu n_*
=\frac{\lambda(b_0^2-1)}{(1+b_0^2)^2}.
$$

Its [eigenvalues](../../../../eigenvalue.md) are $\boxed{-1,\ -\mu}$, both negative, so the positive [equilibrium](../../../../equilibrium-point-of-a-dynamical-system.md) is asymptotically stable against spatially uniform perturbations. This remains true at $\mu=1$, where a repeated [eigenvalue](../../../../eigenvalue.md) may produce a decaying $te^{-t}$ contribution. The printed [stability](../../../../stability-of-a-numerical-method.md) claim must be understood in this spatially uniform sense: sufficiently strong [chemotaxis](../../../../chemotaxis.md) can destabilize nonuniform perturbations, as the next answer shows.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the further mathematical biology course of the University of Oxford](../../../split.md)
5. [Further mathematical biology course of the University of Oxford](../../../../further-mathematical-biology-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
