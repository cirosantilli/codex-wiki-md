<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

For incoming momenta, the Euclidean momentum-space [Feynman rules](../../../../../feynman-rule.md) are

- a $\phi$ propagator $(p^2+m_0^2)^{-1}$;
- a $\chi$ propagator $(p^2+M_0^2)^{-1}$;
- a vertex with two $\phi$ legs and one $\chi$ leg equal to $-\lambda_0(2\pi)^d\delta^{(d)}(p_1+p_2+p_3)$;
- one integration $\int d^d\ell/(2\pi)^d$ for each [loop momentum](../../../../../loop-momentum.md), with division by the [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md).

The one-loop one-particle-irreducible diagrams with at most three external legs can be classified by their external species. There is a one-point $\chi$ [tadpole diagram](../../../../../tadpole-diagram.md) made from a $\phi$ loop. There are two two-point [bubble diagrams](../../../../../bubble-diagram.md): the $\phi$ self-energy has one internal $\phi$ and one internal $\chi$, while the $\chi$ self-energy has two internal $\phi$ lines and symmetry factor $1/2$. For three external legs, three vertices make a triangle: one triangle corrects the $\phi\phi\chi$ vertex and contains two internal $\phi$ lines and one internal $\chi$ line; another has three external $\chi$ legs and a $\phi$ loop, generating a $\chi^3$ interaction. The symmetry $\phi\mapsto-\phi$ forbids amplitudes with an odd number of external $\phi$ legs. The classical $\phi\phi\chi$ vertex is the corresponding tree-level three-point diagram.

Adopt the [self-energy](../../../../../self-energy.md) convention

$$
\widetilde G^{(2)}(p)=\frac1{p^2+m^2-\Pi(p^2)}.
$$

This follows by summing the geometric series of exact propagators separated by amputated one-particle-irreducible two-point insertions. At one loop, after writing $\lambda_0=\mu^{\epsilon/2}\lambda+O(\lambda^3)$,

$$
\Pi_1(p^2)=\lambda^2\mu^\epsilon
\int\frac{d^{6-\epsilon}\ell}{(2\pi)^{6-\epsilon}}
\frac1{(\ell^2+m^2)((\ell+p)^2+M^2)}.
$$

Introduce a [Feynman parameter](../../../../../feynman-parameter.md) and shift the loop momentum. With

$$
\Delta(x)=xm^2+(1-x)M^2+x(1-x)p^2,
$$

[dimensional regularization](../../../../../dimensional-regularization.md) gives

$$
\Pi_1(p^2)=\frac{\lambda^2\mu^\epsilon}{(4\pi)^{3-\epsilon/2}}
\Gamma\left(-1+\frac\epsilon2\right)
\int_0^1dx\,\Delta(x)^{1-\epsilon/2}.
$$

Using $\Gamma(-1+\epsilon/2)=-2/\epsilon+\gamma-1+O(\epsilon)$ produces

$$
\Pi_1(p^2)=\frac1\epsilon(A+Bp^2)+C(p^2,\mu)+O(\epsilon),
$$

where

$$
\boxed{A=-\frac{\lambda^2}{(4\pi)^3}(m^2+M^2),
\qquad B=-\frac{\lambda^2}{3(4\pi)^3}}
$$

and one convenient integral form of the finite part is

$$
\boxed{C(p^2,\mu)=\frac{\lambda^2}{(4\pi)^3}
\int_0^1dx\,\Delta(x)
\left[\log\frac{\Delta(x)}{4\pi\mu^2}+\gamma-1\right]}.
$$

Changing the definition of the dimensional-regularization scale only moves a finite constant between $C$ and the counterterm.

To make the two-point function finite, write $\phi_0=Z_\phi^{1/2}\phi$, express $m_0^2$ in terms of a renormalized mass and a mass counterterm, and choose the pole parts of $\delta Z_\phi$ and $\delta m^2$ to cancel $Bp^2/\epsilon$ and $A/\epsilon$. In the [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md) no additional finite pieces are removed. The physical mass is the [pole mass](../../../../../pole-mass.md), so with the self-energy convention above it obeys

$$
\boxed{m_{\rm phys}^2=m^2(\mu)-\Pi_{\rm MS,fin}(-m_{\rm phys}^2,\mu)}.
$$

The explicit $\mu$ dependence of the finite self-energy cancels the running of $m(\mu)$, leaving $m_{\rm phys}$ independent of the [renormalization scale](../../../../../renormalization-scale.md).

The [superficial degree of divergence](../../../../../superficial-degree-of-divergence.md) counts the ultraviolet power before subdivergences and symmetry cancellations are considered. At $d=6$, a connected graph made from cubic vertices has

$$
D=6L-2I=6-2E,
$$

where $E$ is its number of external legs. Hence one-, two-, and three-point functions can have quartic, quadratic, and logarithmic superficial divergences, whereas graphs with more external legs are superficially convergent.

Full renormalization also requires the $\chi$ mass and wave-function counterterms from its two-point function, a linear $\chi$ counterterm cancelling the tadpole, a coupling counterterm from the divergent $\phi\phi\chi$ triangle, and a $\chi^3$ counterterm from the three-$\chi$ triangle. A vacuum-energy counterterm removes divergent vacuum diagrams. These are precisely the local operators allowed by [power counting in quantum field theory](../../../../../power-counting-in-quantum-field-theory.md) and the exact $\phi\mapsto-\phi$ symmetry.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
