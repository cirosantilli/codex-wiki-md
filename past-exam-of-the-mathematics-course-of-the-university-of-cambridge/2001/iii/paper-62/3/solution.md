<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a connected amputated [Feynman diagram](../../../../../feynman-diagram.md), let $L,I,V,E$ denote its independent loops, internal scalar lines, interaction vertices and external lines. Its [superficial degree of divergence](../../../../../superficial-degree-of-divergence.md) counts the simultaneous ultraviolet scaling of all loop momenta: each loop integration contributes $d$ powers and each [scalar propagator](../../../../../scalar-propagator.md) removes two. A nonderivative interaction adds no numerator powers, so $\Delta=dL-2I$. The graph identities are

$$
nV=2I+E,\qquad L=I-V+1.
$$

The kinetic term gives $[\phi]=(d-2)/2$ and $[\lambda]=d-n(d-2)/2$. Eliminating $I,L$ proves the [monomial scalar interaction power-counting identity](../../../../../monomial-scalar-interaction-power-counting-identity.md):

$$
\boxed{\Delta=d-\frac{d-2}{2}E-[\lambda]V,\qquad\text{order}=\lambda^V.}
$$

For a graph with $C$ connected components the first $d$ is replaced by $dC$, after removing the corresponding overall [momentum](../../../../../momentum.md) delta functions. Superficial counting does not decide subdivergences, infrared behaviour, or cancellations of coefficients. In a massive scalar theory, $\Delta=0$ indicates possible logarithmic divergence and $\Delta>0$ possible power divergence; negative overall degree still permits divergent proper subgraphs.

[Dimensional regularization](../../../../../dimensional-regularization.md) analytically continues the [momentum](../../../../../momentum.md) integration and its angular factors to a complex dimension where a regulated expression is defined, then continues back near the physical dimension. Introduce a scale $\mu$ to keep the renormalized coupling in fixed units. The [minimal subtraction scheme](../../../../../minimal-subtraction-scheme.md) removes only poles in the dimensional regulator, without prescribed finite parts. It differs from [modified minimal subtraction scheme](../../../../../modified-minimal-subtraction-scheme.md), which also absorbs the conventional $\log4\pi-\gamma_E$ combination.

For the cubic calculation, write $g=3!\lambda$, so the interaction is $-g\phi^3/3!$ and the vertex is $-ig$. Use $D=6-2\epsilon$ and the vertex $-ig\mu^\epsilon$. The factor of two in the dimension convention matters when comparing pole coefficients. In six dimensions $[\phi]=2$, $[g]=0$ and a proper two-point graph has $\Delta=2$.

The one-loop [bubble diagram](../../../../../bubble-diagram.md) has [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md) two. Define its amputated insertion $B(p)=i\Pi(p)$ explicitly by

$$
B(p)=\frac{(-ig\mu^\epsilon)^2}{2}\int\frac{d^Dk}{(2\pi)^D}
\frac{i}{k^2-m^2+i0}\frac{i}{(k-p)^2-m^2+i0}.
$$

Combine denominators with a [Feynman parameter](../../../../../feynman-parameter.md) $x$ and shift $\ell=k-xp$. With $M_x^2=m^2-x(1-x)p^2$, the dimensionally continued integral gives

$$
B(p)=\frac{ig^2\mu^{2\epsilon}}{2(4\pi)^{D/2}}\Gamma(2-D/2)
\int_0^1dx\,(M_x^2-i0)^{D/2-2}.
$$

This identity follows by [Wick rotation](../../../../../wick-rotation.md) and a [Schwinger parameterization](../../../../../schwinger-parameterization.md), giving the angular Gaussian factor $(4\pi)^{-D/2}$ and the remaining gamma integral. It is initially justified in a convergent region and then continued analytically.

Here $\Gamma(\epsilon-1)=-1/\epsilon+O(1)$ and $\int_0^1x(1-x)dx=1/6$. Thus the [one-loop two-point divergence in six-dimensional cubic scalar theory](../../../../../one-loop-two-point-divergence-in-six-dimensional-cubic-scalar-theory.md) is

$$
\boxed{B_{\rm div}(p)=-\frac{ig^2}{2(4\pi)^3\epsilon}\left(m^2-\frac{p^2}{6}\right)
=-\frac{18i\lambda^2}{(4\pi)^3\epsilon}\left(m^2-\frac{p^2}{6}\right).}
$$

Writing $\Delta_0(p)=i/(p^2-m^2+i0)$, the proper-bubble contribution to the [propagator](../../../../../propagator.md) is

$$
\boxed{(\Delta_0B\Delta_0)_{\rm div}
=\frac{ig^2(m^2-p^2/6)}{2(4\pi)^3\epsilon(p^2-m^2+i0)^2}.}
$$

With the defined $B=i\Pi$, resummation gives $i/(p^2-m^2+\Pi+i0)$. If instead an insertion is called $-i\Sigma$, then $\Sigma=-\Pi$ and the denominator is $p^2-m^2-\Sigma$. These naming conventions must not reverse the calculated graph.

For example, the [minimal-subtraction two-point counterterms in cubic scalar theory](../../../../../minimal-subtraction-two-point-counterterms-in-cubic-scalar-theory.md) can be written

$$
\mathcal L_{\rm ct}=\frac12\delta Z(\partial\phi)^2-\frac12\delta m^2\phi^2,
\qquad
\boxed{\delta Z=-\frac{g^2}{12(4\pi)^3\epsilon},\quad
\delta m^2=-\frac{g^2m^2}{2(4\pi)^3\epsilon}.}
$$

Their insertion $i(\delta Zp^2-\delta m^2)$ cancels the bubble pole. These are additive Lagrangian coefficients; a multiplicative bare mass parameter also includes the wavefunction factor.

There is a vacuum convention to specify because a cubic interaction does not preserve a zero mean field automatically. If no [tadpole subtraction](../../../../../tadpole-subtraction.md) or background shift is imposed, a connected [two-point function](../../../../../two-point-correlation-function.md) also has a one-particle-reducible one-loop graph with both external legs at one cubic vertex and a [tadpole diagram](../../../../../tadpole-diagram.md) attached to its third leg. For $m>0$, the amputated one-point [tadpole diagram](../../../../../tadpole-diagram.md) is

$$
T_1=\frac{-ig\mu^\epsilon}{2}\int\frac{d^Dk}{(2\pi)^D}\frac{i}{k^2-m^2+i0},
\qquad (T_1)_{\rm div}=-\frac{igm^4}{4(4\pi)^3\epsilon}.
$$

This uses $\Gamma(\epsilon-2)=1/(2\epsilon)+O(1)$. Its mean-field pole is $v_{\rm div}=\Delta_0(0)(T_1)_{\rm div}=-gm^2/[4(4\pi)^3\epsilon]$. The [tadpole contribution to a cubic-theory two-point function](../../../../../tadpole-contribution-to-a-cubic-theory-two-point-function.md) is therefore

$$
B_{{\rm tad},\rm div}=(-ig)v_{\rm div}=\frac{ig^2m^2}{4(4\pi)^3\epsilon}.
$$

In that unshifted convention, the total connected one-loop [propagator](../../../../../propagator.md) pole is

$$
\boxed{\Delta_{{\rm conn},\rm div}^{(1)}(p)
=\frac{ig^2(m^2/2-p^2/6)}{2(4\pi)^3\epsilon(p^2-m^2+i0)^2}.}
$$

A linear [counterterm](../../../../../counterterm.md) imposing $\langle\phi\rangle=0$ cancels the attached [tadpole diagram](../../../../../tadpole-diagram.md), leaving the usual proper-bubble result above. [Vacuum bubbles](../../../../../vacuum-feynman-diagram.md) cancel by normalization. A disconnected product $\langle\phi\rangle^2$ belongs to the unconnected [two-point function](../../../../../two-point-correlation-function.md) and has two [tadpole diagram](../../../../../tadpole-diagram.md) loops, so it is outside the requested connected one-loop [propagator](../../../../../propagator.md) correction. In the massless theory, isolated [tadpole diagrams](../../../../../tadpole-diagram.md) are scaleless and vanish in [dimensional regularization](../../../../../dimensional-regularization.md); an infrared-safe nonzero external scale is still needed to distinguish ultraviolet poles from scaleless integrals.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 62](../../paper-62-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
