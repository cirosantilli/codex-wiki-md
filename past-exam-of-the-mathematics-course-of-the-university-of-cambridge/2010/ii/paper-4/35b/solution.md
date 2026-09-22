<h1 id="35b/solution">Solution</h1>

↑ **Parent:** [35B](../35b.md)

Write the superconducting order parameter as $\psi=\sqrt{n_s}e^{i\vartheta}$, with carrier mass $m$. Minimal electromagnetic coupling gives mechanical momentum $\hbar\nabla\vartheta-q\mathbf A$, so the current density is

$$
\boxed{\mathbf j=\frac{n_sq}{m}
(\hbar\nabla\vartheta-q\mathbf A).}
$$

It also follows by substituting $\psi$ into $(q\hbar/m)\operatorname{Im}(\psi^*\nabla\psi)-(q^2/m)|\psi|^2\mathbf A$. In a gauge where the phase is constant, this reduces to the [London equation](../../../../../london-equations.md) $\mathbf j=-n_sq^2\mathbf A/m$.

Under $\mathbf A\mapsto\mathbf A+\nabla\chi$, the phase changes by $\vartheta\mapsto\vartheta+q\chi/\hbar$. The two gradient changes cancel, proving [gauge invariance](../../../../../gauge-invariance.md) of the actual current. A formula omitting the phase term is valid only in its chosen gauge.

For a uniform superconductor without vortices, taking a curl gives $\nabla\times\mathbf j=-n_sq^2\mathbf B/m$. Combine this with the stationary [Ampère's law](../../../../../ampere-s-circuital-law.md) $\nabla\times\mathbf B=\mu_0\mathbf j$ and $\nabla\cdot\mathbf B=0$ to obtain

$$
\nabla^2\mathbf B=\frac{\mathbf B}{\lambda_L^2},
\qquad \lambda_L=\sqrt{\frac{m}{\mu_0n_sq^2}}.
$$

For a [magnetic field](../../../../../magnetic-field.md) parallel to the planar interface, translation [symmetry](../../../../../symmetry-physics.md) reduces the equation to $\mathbf B''=\mathbf B/\lambda_L^2$. Boundedness and decay as $z\to\infty$, together with the tangential boundary value, give the [Meissner effect](../../../../../meissner-effect.md)

$$
\boxed{\mathbf B(z)=\mathbf B_0e^{-z/\lambda_L},\qquad z>0.}
$$

Here $\lambda_L$ is the [London penetration depth](../../../../../london-penetration-depth.md).

The parallel-field assumption is necessary for this one-dimensional Meissner solution. If the printed arbitrary constant $\mathbf B_0$ has a nonzero normal component, $\nabla\cdot\mathbf B=0$ forces that component to be constant across a translation-invariant half-space, whereas the [London equation](../../../../../london-equations.md) forces it to vanish. Thus no decaying planar Meissner state with that boundary value exists; one must change the geometry or allow a different magnetic state.

## ↑ Ancestors (10)

1. [35B](../35b.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
