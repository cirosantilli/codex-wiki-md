<h1 id="11c/solution">Solution</h1>

↑ **Parent:** [11C](../11c.md)

For a Cartesian [change of basis](../../../../../change-of-basis.md) represented by an [orthogonal matrix](../../../../../orthogonal-matrix.md) $Q$, [vectors](../../../../../vector.md) transform as $E'_i=Q_{ia}E_a$ and $B'_i=Q_{ia}B_a$. Their squared norms are invariant and $Q_{ia}Q_{jb}\delta_{ab}=\delta_{ij}$. Substitution into the given expression therefore gives

$$
\boxed{T'_{ij}=Q_{ia}Q_{jb}T_{ab},}
$$

the transformation law of a [Cartesian second-rank tensor](../../../../../cartesian-second-rank-tensor.md). The [magnetic field](../../../../../magnetic-field.md)'s extra axial sign under an improper physical reflection, if included, appears twice and cancels in its quadratic contribution.

Write the [Maxwell stress tensor](../../../../../maxwell-stress-tensor.md) as $T=\mathbf E\mathbf E+\mathbf B\mathbf B-\tfrac12(E^2+B^2)I$. Its [divergence](../../../../../divergence.md) is

$$
\mathbf M=(\mathbf E\cdot\nabla)\mathbf E+\mathbf E\nabla\cdot\mathbf E
+(\mathbf B\cdot\nabla)\mathbf B+\mathbf B\nabla\cdot\mathbf B
-\tfrac12\nabla(E^2+B^2).
$$

The identity $(\mathbf A\cdot\nabla)\mathbf A-\tfrac12\nabla A^2=-\mathbf A\times(\nabla\times\mathbf A)$ follows by contracting two [Levi-Civita symbols](../../../../../levi-civita-symbol.md), or directly by differentiating components. Using [Maxwell's equations](../../../../../maxwell-equations.md) consequently yields

$$
\begin{aligned}
\mathbf M
&=\rho\mathbf E-\mathbf E\times(\nabla\times\mathbf E)-\mathbf B\times(\nabla\times\mathbf B)\\
&=\rho\mathbf E+\mathbf E\times\mathbf B_t-\mathbf B\times(\mathbf J+\mathbf E_t)\\
&=\rho\mathbf E+\mathbf J\times\mathbf B+\partial_t(\mathbf E\times\mathbf B).
\end{aligned}
$$

Hence the [local conservation of electromagnetic momentum](../../../../../local-conservation-of-electromagnetic-momentum.md) is

$$
\boxed{\partial_t(\mathbf E\times\mathbf B)=\mathbf M-\rho\mathbf E-\mathbf J\times\mathbf B,
\qquad M_i=\partial_jT_{ij}.}
$$

The two subtracted terms are the [Lorentz force density](../../../../../lorentz-force-density.md), while $\mathbf E\times\mathbf B$ is the [electromagnetic momentum density](../../../../../electromagnetic-momentum-density.md) in the units used here.

## ↑ Ancestors (10)

1. [11C](../11c.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
