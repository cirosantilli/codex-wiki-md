<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let the charge parameter depend on position temporarily. Using the [gauge-covariant derivative of a charged scalar field](../../../../../gauge-covariant-derivative-of-a-charged-scalar-field.md), the variation of the matter action is $\delta S=\int d^4x\,j^\mu\partial_\mu\alpha$. The resulting [Noether current](../../../../../noether-current.md) is

$$
\boxed{j^\mu=i\bigl[\phi\,\nabla^\mu\bar\phi-\bar\phi\,\nabla^\mu\phi\bigr]=i(\phi\partial^\mu\bar\phi-\bar\phi\partial^\mu\phi)-2A^\mu|\phi|^2.}
$$

Here $\nabla_\mu\bar\phi=\partial_\mu\bar\phi+iA_\mu\bar\phi$. The potential does not contribute, and $j^\mu=-\delta S_{\mathrm{matter}}/\delta A_\mu$. Because $A$ has not been rescaled to a canonical [kinetic term](../../../../../kinetic-term.md), there is no factor $e$ in this [Noether current](../../../../../noether-current.md) or in the matter [interaction vertices](../../../../../interaction-vertex.md).

A local change of variables in the [path integral](../../../../../path-integral.md) gives $\delta\langle\phi(y)\bar\phi(z)\rangle=\langle\delta(\phi(y)\bar\phi(z))-(\delta S)\phi(y)\bar\phi(z)\rangle=0$. [Integration by parts](../../../../../integration-by-parts.md) in the term containing $\partial\alpha$ produces the two opposite contact terms of the [Ward identity](../../../../../ward-identity.md).

For clarity about phases, transform the current correlator with $e^{i(p-p')\cdot x-ip\cdot y+ip'\cdot z}$ and suppress its overall [momentum conservation](../../../../../momentum-conservation.md) [Dirac delta function](../../../../../dirac-delta-function.md). Denote the result by $C^\mu(p,p')$. The coordinate [Ward identity](../../../../../ward-identity.md) becomes

$$
-i(p-p')_\mu C^\mu=-i\Delta(p')+i\Delta(p),\qquad
(p-p')_\mu C^\mu=\Delta(p')-\Delta(p).
$$

[Amputation](../../../../../amputation-of-external-propagators.md) of the two external [quantum field theory propagators](../../../../../propagator.md) then fixes the longitudinal part of the current [interaction vertex](../../../../../interaction-vertex.md). Since the action couples $A_\mu$ to $-j^\mu$, the gauge [interaction vertex](../../../../../interaction-vertex.md) has the opposite sign. The phase convention for the paper's gauge [interaction vertices](../../../../../interaction-vertex.md) is $\Gamma^\mu=iG^\mu$, where $G^\mu$ is the corresponding derivative of the Euclidean [quantum effective action](../../../../../effective-action.md).

One can derive the exact [one-particle-irreducible correlation function](../../../../../one-particle-irreducible-correlation-function.md) directly, without assuming the entire connected current correlator is one-particle irreducible. Local [gauge invariance](../../../../../gauge-invariance.md) of the [quantum effective action](../../../../../effective-action.md) implies

$$
\partial_\mu\frac{\delta\Gamma_{\mathrm{eff}}}{\delta A_\mu(x)}=i\phi(x)\frac{\delta\Gamma_{\mathrm{eff}}}{\delta\phi(x)}-i\bar\phi(x)\frac{\delta\Gamma_{\mathrm{eff}}}{\delta\bar\phi(x)}.
$$

A linear covariant [gauge fixing](../../../../../gauge-fixing.md) adds a breaking term independent of the scalars, which disappears after the scalar differentiations below. The identity requires a [regularization in quantum field theory](../../../../../regularization-in-quantum-field-theory.md) and [counterterms](../../../../../counterterm.md) preserving the [Abelian gauge theory](../../../../../abelian-gauge-theory.md) [Ward identity](../../../../../ward-identity.md); [scalar quantum electrodynamics](../../../../../scalar-electrodynamics.md) has no [gauge anomaly](../../../../../gauge-anomaly.md).

Differentiate with respect to $\phi(y)$ and $\bar\phi(z)$, then set all background fields to zero. The two-point derivative is the inverse exact [quantum field theory propagator](../../../../../propagator.md). Use the [Fourier transform](../../../../../fourier-transform.md) convention $\phi(x)=\int_p e^{ip\cdot x}\phi(p)$, $\bar\phi(x)=\int_{p'}e^{-ip'\cdot x}\bar\phi(p')$, with the photon momentum $p'-p$ incoming. This gives

$$
(p-p')_\mu G^\mu(p,p')=\Delta(p')^{-1}-\Delta(p)^{-1},
\qquad
\boxed{(p-p')_\mu\Gamma^\mu(p,p')=i[\Delta(p')^{-1}-\Delta(p)^{-1}].}
$$

At tree level $G^\mu=-(p+p')^\mu$, so $\Gamma^\mu=-i(p+p')^\mu$, and the identity reduces to $-i(p^2-p'^2)=i(p'^2-p^2)$.

To obtain the [two-photon scalar Ward identity](../../../../../two-photon-scalar-ward-identity.md), differentiate the same functional [Ward identity](../../../../../ward-identity.md) also with respect to $A_\nu(w)$. In terms of Euclidean action derivatives it reads

$$
\partial_x^\mu G_{\mu\nu}(x,w;y,z)=i\delta^4(x-y)G_\nu(w;x,z)-i\delta^4(x-z)G_\nu(w;y,x).
$$

This construction automatically includes the [seagull vertex](../../../../../seagull-vertex.md): the [Noether current](../../../../../noether-current.md) depends on $A$, with $\delta j^\mu(x)/\delta A_\nu(w)=-2\delta^{\mu\nu}\delta^4(x-w)|\phi(x)|^2$. It cannot be discarded when differentiating a current insertion.

Take the first photon momentum to be incoming $k$, and the second incoming $p'-p-k$. On the first scalar leg the contact term shifts $p$ to $p+k$; on the other it shifts $p'$ to $p'-k$. Consequently

$$
k_\mu G^{\mu\nu}(k;p,p')=G^\nu(p,p'-k)-G^\nu(p+k,p').
$$

With $\Gamma^{\mu\nu}=i^2G^{\mu\nu}=-G^{\mu\nu}$, the result is

$$
\boxed{k_\mu\Gamma^{\mu\nu}(k;p,p')=i\Gamma^\nu(p,p'-k)-i\Gamma^\nu(p+k,p').}
$$

**There is a momentum-routing sign error in the printed second identity.** With the scalar momentum convention of the first identity, its first shifted argument must be $p'-k$, not $k-p'$. This is already forced at tree level: the [seagull vertex](../../../../../seagull-vertex.md) has $G^{\mu\nu}=2\delta^{\mu\nu}$ and hence $\Gamma^{\mu\nu}=-2\delta^{\mu\nu}$. The corrected right-hand side is $-2k^\nu$, matching the left-hand side, whereas the printed right-hand side is $-2p'^\nu$. Changing to an all-incoming scalar convention would also change the first identity, so it does not fix both printed formulas simultaneously.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 304](../../paper-304-split.md)
3. [Iii](../../split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
