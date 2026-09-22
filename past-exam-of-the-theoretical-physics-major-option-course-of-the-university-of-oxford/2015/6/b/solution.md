<h1 id="6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Define the free [Feynman propagators](../../../../feynman-propagator.md) by

$$
D_0(x)=\int\frac{d^4k}{(2\pi)^4}\frac{i\,e^{-ik\cdot x}}{k^2+i0},\qquad
D_m(x)=\int\frac{d^4k}{(2\pi)^4}\frac{i\,e^{-ik\cdot x}}{k^2-m^2+i0}.
$$

The interaction preserves the global phase symmetry $\varphi\mapsto e^{i\alpha}\varphi$, with the real $\phi$ neutral. Therefore the charge-two correlator vanishes in a symmetry-invariant perturbative vacuum:

$$
\boxed{\langle T\varphi(x)\varphi(y)\phi(z)\rangle=0.}
$$

In [Wick contractions](../../../../wick-contraction.md), a complex field contracts only with its conjugate; one vertex has one of each and cannot absorb both external $\varphi$ fields. The symmetry shows this vanishing holds to all perturbative orders, not only first order.

The neutral connected correlator has one allowed contraction to each external point at order $g$:

$$
\boxed{G_{\rm conn}(x,y,z)=-ig\int d^4w\,
D_0(x-w)D_0(y-w)D_m(z-w)+O(g^3).}
$$

The propagators are even functions of their separation; their orientations encode the conjugate-field contractions. Equivalently, with every external momentum Fourier transformed as incoming,

$$
G_{\rm conn}(x,y,z)=(-ig)\int\frac{d^4k\,d^4\ell\,d^4r}{(2\pi)^{12}}
(2\pi)^4\delta^{(4)}(k+\ell+r)e^{-i(kx+\ell y+rz)}
\frac{i}{k^2+i0}\frac{i}{\ell^2+i0}\frac{i}{r^2-m^2+i0}+O(g^3).
$$

No factor of two accompanies the vertex: $\varphi$ and $\varphi^\dagger$ are distinct fields.

**For the full correlator as literally written, a [disconnected scalar three-point tadpole](../../../../disconnected-scalar-three-point-tadpole.md) is also possible.** Contract the two external complex fields with each other and contract the complex pair at the vertex into a loop. Unless [normal ordering](../../../../normal-ordering.md) is imposed on the interaction or a [tadpole counterterm](../../../../tadpole-counterterm.md) fixes $\langle\phi\rangle=0$, add

$$
\boxed{G_{\rm disc}(x,y,z)=D_0(x-y)\left[-igD_0(0)\int d^4w\,D_m(z-w)\right]+O(g^3).}
$$

The coincident propagator is regulator dependent; in [dimensional regularization](../../../../dimensional-regularization.md) the massless scaleless [tadpole diagram](../../../../tadpole-diagram.md) vanishes. More generally this is $\langle T\varphi^\dagger(x)\varphi(y)\rangle_0\langle\phi(z)\rangle$ to this order and is removed by taking the connected correlator or imposing the stated vacuum-renormalization condition. Normalizing by vacuum bubbles alone does not remove an external-leg disconnected [tadpole diagram](../../../../tadpole-diagram.md). The charged correlator remains zero in every one of these conventions.[§§3.3.2 and 3.7.1, Wick expansion, connected Green functions and vacuum normalization](../../../../quantum-field-theory-by-david-tong.md)

## ↑ Ancestors (12)

1. [B](../b.md)
2. [6](../../6.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the theoretical physics major option course of the University of Oxford](../../../split.md)
5. [Theoretical physics major option course of the University of Oxford](../../../../theoretical-physics-major-option-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
