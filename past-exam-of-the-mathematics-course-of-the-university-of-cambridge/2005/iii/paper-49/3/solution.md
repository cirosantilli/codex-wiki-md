<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Split the free [interaction picture](../../../../../interaction-picture.md) field as $\phi=\phi^{(+)}+\phi^{(-)}$, where the first part contains [annihilation operators](../../../../../annihilation-operator.md) and the second [creation operators](../../../../../creation-operator.md). [Time ordering](../../../../../time-ordering.md) places the operator at the later time on the left, while [normal ordering](../../../../../normal-ordering.md) places all [creation operators](../../../../../creation-operator.md) on the left. For $x^0>y^0$, commuting the annihilation part of the first field through the creation part of the second gives

$$
\phi(x)\phi(y)=:\phi(x)\phi(y):+[\phi^{(+)}(x),\phi^{(-)}(y)].
$$

The [commutator](../../../../../commutator.md) is the c-number

$$
[\phi^{(+)}(x),\phi^{(-)}(y)]
=\int\frac{d^3p}{(2\pi)^3}\frac{e^{-ip\cdot(x-y)}}{2E_{\mathbf p}}.
$$

For $y^0>x^0$, the same calculation interchanges $x,y$. Combining the two time orders proves the [two-field Wick contraction identity](../../../../../two-field-wick-contraction-identity.md)

$$
\boxed{T\phi(x)\phi(y)=:\phi(x)\phi(y):+D_F(x-y)},
$$

where

$$
D_F(x-y)=\langle0|T\phi(x)\phi(y)|0\rangle
=\int\frac{d^4p}{(2\pi)^4}\frac{i\,e^{-ip\cdot(x-y)}}{p^2-m^2+i0}.
$$

The equality with the four-dimensional integral follows by closing the energy contour at the positive-energy pole for $x^0>y^0$ and the negative-energy pole for the reverse order. This fixes the [scalar Feynman propagator pole prescription](../../../../../scalar-feynman-propagator-pole-prescription.md); in this convention $D_F$ itself includes the factor $i$.

Because these interactions have no derivatives, $H_{\rm int}=-\int\mathcal L_{\rm int}d^3x$. Expand the [Dyson series](../../../../../dyson-series.md)

$$
S=T\exp\left(i\int d^4z\left[\frac{\mu}{3!}\phi(z)^3-\frac{\lambda}{4!}\phi(z)^4\right]\right).
$$

Apply the [Wick theorem](../../../../../wick-s-theorem.md) to each term together with the external insertions. Every paired field contributes a propagator, and the remaining normal-ordered vacuum expectation vanishes unless no fields remain. Representing the propagators by Fourier integrals and integrating each vertex position gives the [four-momentum conservation](../../../../../four-momentum-conservation.md) delta function. The $3!$ and $4!$ contractions into labelled vertex slots cancel the factorials in the interaction density. The resulting [scalar-field cubic and quartic Feynman vertices](../../../../../scalar-field-cubic-and-quartic-feynman-vertices.md) are

$$
\boxed{\text{propagator: }\frac{i}{p^2-m^2+i0},\qquad
\text{cubic vertex: }i\mu,\qquad
\text{quartic vertex: }-i\lambda}.
$$

Each vertex also has $(2\pi)^4\delta^{(4)}(\sum p)$, each independent internal [momentum](../../../../../momentum.md) is integrated with $d^4p/(2\pi)^4$, and repeated equivalent contractions give the usual [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md). For the unamputated correlation functions, retain the propagators joining external insertions to vertices. The displayed unnormalized numerator includes disconnected [vacuum bubbles](../../../../../vacuum-feynman-diagram.md); dividing by $\langle0|S|0\rangle$ cancels them. Amputated [scattering amplitudes](../../../../../scattering-amplitude.md) additionally use the [LSZ reduction formula](../../../../../lsz-reduction-formula.md).

For stability, examine the classical [scalar potential](../../../../../scalar-potential.md)

$$
V(\phi)=\frac12m^2\phi^2-\frac{\mu}{6}\phi^3+\frac{\lambda}{24}\phi^4.
$$

The tree-level boundedness criterion is **$\lambda>0$**, with arbitrary real cubic coupling. If $\lambda=0$, boundedness requires $\mu=0$ and $m^2\ge0$; if $\lambda<0$, or $\lambda=0$ with $\mu\ne0$, the potential is unbounded below. Thus a positive quartic coupling permits a stable ground-state vacuum, although it need not be the perturbative vacuum at $\phi=0$.

For $\lambda>0$ and $m^2\ge0$, the [stability of a cubic-quartic scalar potential](../../../../../stability-of-a-cubic-quartic-scalar-potential.md) determines when zero is a global minimum:

$$
V(\phi)=\phi^2\left[\frac{\lambda}{24}\left(\phi-\frac{2\mu}{\lambda}\right)^2
+\frac{m^2}{2}-\frac{\mu^2}{6\lambda}\right].
$$

The square bracket is nonnegative for every field value exactly when

$$
\boxed{\mu^2\le3\lambda m^2}.
$$

For a nontrivial equality case there is a second degenerate minimum at $\phi=2\mu/\lambda$. If $m^2>0$ and $\mu^2>3\lambda m^2$, zero remains a local minimum but is a [false vacuum](../../../../../false-vacuum.md), with a lower minimum elsewhere. If $m^2=\mu=0$ and $\lambda>0$, the origin is the quartic minimum despite its vanishing quadratic curvature. These are classical or tree-level stability statements; renormalized couplings and the [quantum effective potential](../../../../../quantum-effective-potential.md) refine the quantum analysis.

<a id="3/image-stable-degenerate-and-metastable-scalar-vacua"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-49-scalar-vacua.png)

**[Figure 1](#3/image-stable-degenerate-and-metastable-scalar-vacua). Stable, degenerate and metastable scalar vacua**.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 49](../../paper-49-split.md)
3. [Iii](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
