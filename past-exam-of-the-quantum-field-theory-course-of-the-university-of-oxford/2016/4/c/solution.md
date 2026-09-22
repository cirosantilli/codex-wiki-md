<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

It is convenient to evaluate the [one-particle irreducible](../../../../one-particle-irreducible-feynman-diagram.md) vertices using the [Euclidean action](../../../../euclidean-action.md) and then translate the [counterterms](../../../../counterterm.md) back to the [Minkowski spacetime](../../../../minkowski-spacetime.md) [Lagrangian density](../../../../lagrangian-density.md). For the [tadpole integral](../../../../tadpole-integral.md), [analytic continuation](../../../../analytic-continuation.md) of [solution](../b/solution.md) gives

$$
I_{D,1}=\frac{\Gamma(-1+\epsilon/2)}{(4\pi)^{2-\epsilon/2}}(m^2)^{1-\epsilon/2}
=-\frac{m^2}{8\pi^2\epsilon}+O(1).
$$

Indeed $\Gamma(-1+\epsilon/2)=\Gamma(\epsilon/2)/(\epsilon/2-1)=-2/\epsilon+O(1)$. The negative pole is a property of [analytic continuation](../../../../analytic-continuation.md), not the value of a convergent positive integral.

The [Euclidean space](../../../../euclidean-norm.md) inverse two-point [vertex](../../../../vertex-graph-theory.md) has the one-loop correction

$$
\Gamma_E^{(2)}(p_E)=p_E^2+m^2+\frac{\lambda_0}{2}I_{D,1}+O(\lambda_0^2),
\qquad
\left.\Gamma_E^{(2)}\right|_{\rm pole}=-\frac{\lambda_0m^2}{16\pi^2\epsilon}.
$$

The factor $1/2$ is the [symmetry factor](../../../../feynman-diagram-symmetry-factor.md) weight of the [tadpole diagram](../../../../tadpole-diagram.md). A mass [counterterm](../../../../counterterm.md) $\delta m^2=\lambda_0m^2/(16\pi^2\epsilon)$ cancels this pole. There is no momentum-dependent pole at this order, and hence no one-loop [wave-function renormalization](../../../../wave-function-renormalization.md).

For the four-point [vertex](../../../../vertex-graph-theory.md), the three [bubble diagrams](../../../../bubble-diagram.md) give

$$
\Gamma_E^{(4)}=\lambda_0-\frac{\lambda_0^2}{2}(B_s+B_t+B_u)+O(\lambda_0^3),
\qquad
\left.\Gamma_E^{(4)}\right|_{\rm pole}=-\frac{3\lambda_0^2}{16\pi^2\epsilon}.
$$

One can check the relative minus sign independently from the one-loop [effective action](../../../../effective-action.md): its $\tfrac12\operatorname{Tr}\log(1+G\lambda_0\phi^2/2)$ term has a positive term linear in $\lambda_0\phi^2$ and a negative term quadratic in it. Thus $\delta\lambda=3\lambda_0^2/(16\pi^2\epsilon)$ cancels the quartic pole.

In the [Euclidean action](../../../../euclidean-action.md), these two [counterterms](../../../../counterterm.md) are $+\delta m^2\phi^2/2+\delta\lambda\phi^4/4!$. Returning to the [Minkowski spacetime](../../../../minkowski-spacetime.md) [Lagrangian density](../../../../lagrangian-density.md) gives

$$
\boxed{\mathcal L_{\rm ct}=-\frac12\frac{\lambda_0m^2}{16\pi^2\epsilon}\phi^2
-\frac1{4!}\frac{3\lambda_0^2}{16\pi^2\epsilon}\phi^4.}
$$

For a direct sign check with [Feynman rules](../../../../feynman-rules.md), the two amputated loop pole insertions are $+i\lambda_0m^2/(16\pi^2\epsilon)$ and $+i3\lambda_0^2/(16\pi^2\epsilon)$, while the [counterterm](../../../../counterterm.md) insertions are $-i\delta m^2$ and $-i\delta\lambda$.

As usual, the displayed pole residues suppress [renormalization scale](../../../../renormalization-scale.md) powers: $[\lambda_0]=\epsilon$ away from four dimensions. The next part restores these powers explicitly with a dimensionless [renormalized coupling](../../../../renormalized-coupling.md). Replacing the tree coupling by its renormalized counterpart inside a one-loop residue changes only higher-loop terms.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [4](../../4.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the quantum field theory course of the University of Oxford](../../../split.md)
5. [Quantum field theory course of the University of Oxford](../../../../quantum-field-theory-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)

## ← Incoming links (1)

- [Solution](../d/solution.md)
