<h1 id="3/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

At order $e^2$, scalar particle–[antiparticle](../../../../../../antiparticle.md) scattering has a $t$-channel photon exchange and an $s$-channel annihilation and recreation diagram. They are shown below, with incoming momenta $p,q$ and outgoing momenta $p',q'$. The [seagull vertex](../../../../../../seagull-vertex.md) has only two scalar legs and does not yield a four-scalar tree diagram at this order.

<a id="3/d/image-leading-scalar-particle-antiparticle-scattering-diagrams-with-exchanged-and-annihilation-channel-photons"></a>
![](../../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-50-scalar-qed-tree.png)

**[Figure 2](#3/d/image-leading-scalar-particle-antiparticle-scattering-diagrams-with-exchanged-and-annihilation-channel-photons). Leading scalar particle–antiparticle scattering diagrams with exchanged and annihilation-channel photons**.

For the exchange graph, let $k=p-p'=q'-q$. Apart from overall charge signs, the two scalar currents are $J=p+p'$ and $K=q+q'$. The external [mass shell](../../../../../../mass-shell.md) conditions give

$$
k\cdot J=p^2-p'^2=0,\qquad k\cdot K=q'^2-q^2=0.
$$

For the annihilation graph, $k=p+q=p'+q'$, with currents $J=p-q$ and $K=p'-q'$, again up to vertex signs. Their contractions are $p^2-q^2=0$ and $p'^2-q'^2=0$. Thus each graph couples the photon to [conserved currents](../../../../../../conserved-current.md), the relevant [scalar quantum electrodynamics Ward identity](../../../../../../scalar-quantum-electrodynamics-ward-identity.md).

Write $k=(\omega,\mathbf k)$ and $\kappa^2=|\mathbf k|^2$. [conserved current](../../../../../../conserved-current.md) means $\mathbf k\cdot\mathbf J=\omega J^0$ and $\mathbf k\cdot\mathbf K=\omega K^0$. For $\kappa\ne0$, contraction with the [Coulomb-gauge photon propagator](../../../../../../coulomb-gauge-photon-propagator.md) gives, displaying the rational identity before the pole boundary limit,

$$
\begin{aligned}
J^\mu D^{\mathrm C}_{\mu\nu}K^\nu
&=\frac{iJ^0K^0}{\kappa^2}
+\frac{i}{k^2}\left(\mathbf J\cdot\mathbf K-\frac{(\mathbf J\cdot\mathbf k)(\mathbf K\cdot\mathbf k)}{\kappa^2}\right)\\
&=\frac{i\mathbf J\cdot\mathbf K}{k^2}
+\frac{iJ^0K^0}{\kappa^2}\left(1-\frac{\omega^2}{k^2}\right)\\
&=\frac{i}{k^2}\bigl(\mathbf J\cdot\mathbf K-J^0K^0\bigr)
=-\frac{i}{k^2}J\cdot K.
\end{aligned}
$$

We used $k^2=\omega^2-\kappa^2$. Restoring the common [Feynman i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) yields the [Coulomb-gauge propagator between conserved currents](../../../../../../coulomb-gauge-propagator-between-conserved-currents.md) result

$$
\boxed{J^\mu D^{\mathrm C}_{\mu\nu}K^\nu
=J^\mu\left(\frac{-i\eta_{\mu\nu}}{k^2+i0}\right)K^\nu.}
$$

Hence each on-shell tree amplitude can use the Lorentz-invariant propagator. This is equality after contraction, not equality of the gauge-dependent tensors. At $\mathbf k=0$, the separate Coulomb-gauge terms are ill-defined; combine them first and take the conserved-current limit. The combined expression has only the physical photon pole.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [3](../../3.md)
3. [Paper 50](../../../paper-50-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
