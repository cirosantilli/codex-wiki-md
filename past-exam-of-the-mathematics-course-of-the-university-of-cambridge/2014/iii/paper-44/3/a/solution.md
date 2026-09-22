<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Fix the sign convention by taking the proper two-point insertion to be $i\Sigma(\not p)$. This convention matches the loop expression and mass conversion printed later. [Dyson resummation](../../../../../../dyson-resummation.md) of successive [fermion self-energy](../../../../../../fermion-self-energy.md) insertions gives

$$
iG=\frac{i}{\not p-m}+\frac{i}{\not p-m}(i\Sigma)\frac{i}{\not p-m}+\cdots
=\boxed{\frac{i}{\not p-m+\Sigma_R(\not p)}}.
$$

The subscript denotes the renormalized [self-energy](../../../../../../self-energy.md). If the insertion is instead named $-i\Sigma_{\rm usual}$, then $\Sigma_{\rm usual}=-\Sigma_R$ and the denominator is written $\not p-m-\Sigma_{\rm usual}$. These are the same physical convention.

[Lorentz covariance](../../../../../../lorentz-covariance.md) allows $\Sigma_R=\mathcal A(p^2)\not p+\mathcal B(p^2)m$. The physical mass-shell condition is

$$
\boxed{[1+\mathcal A(m_{\rm phys}^2)]m_{\rm phys}
-[1-\mathcal B(m_{\rm phys}^2)]m=0.}
$$

It locates the mass-shell singularity of the [Dirac propagator](../../../../../../dirac-propagator.md). In infrared-regulated perturbation theory this is the [pole mass](../../../../../../pole-mass.md); near a simple pole the [quantum field theory propagator](../../../../../../propagator.md) has the form $iZ_{\rm pole}(\not p+m_{\rm phys})/(p^2-m_{\rm phys}^2+i0)$. The mass and pole residue are different quantities: the former fixes the singularity's location, the latter the field normalization. The calculation below uses this standard perturbative pole-mass definition.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 44](../../../paper-44-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
