<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the momentum-space [Feynman rules](../../../../../feynman-rule.md) with the scalar [Feynman propagator](../../../../../feynman-propagator.md) $i/(p^2-m^2+i0)$. The [four-leg vertex of a factorial-normalized scalar interaction](../../../../../four-leg-vertex-of-a-factorial-normalized-scalar-interaction.md) has weight **$i\lambda$** for the positive interaction sign printed here. There are $4!$ [Wick contractions](../../../../../wick-contraction.md) assigning four external legs to its four fields, cancelling the factorial in its coefficient. A negative interaction sign would give $-i\lambda$; its squared tree amplitude is the same.

At each vertex include $(2\pi)^4\delta^4(\sum p)$ with all incident momenta taken incoming. Assign an internal momentum to each line and integrate each independent loop with $\int d^4\ell/(2\pi)^4$. Divide a graph by its [Feynman-diagram symmetry factor](../../../../../feynman-diagram-symmetry-factor.md), sum the graphs at the chosen order, and omit disconnected vacuum graphs from normalized amplitudes. For an [S-matrix](../../../../../s-matrix.md) element, amputate external propagators and put the external momenta on shell as in the [LSZ reduction formula](../../../../../lsz-reduction-formula.md); the external one-particle residues are one at tree level.

Define the invariant amplitude by the relativistically normalized matrix element

$$
\langle p_3p_4|S-1|p_1p_2\rangle=i(2\pi)^4\delta^4(p_1+p_2-p_3-p_4)\,\mathcal M,
$$

with $\langle p|p'\rangle=2E_{\mathbf p}(2\pi)^3\delta^3(\mathbf p-\mathbf p')$. The lowest-order connected four-point graph is one contact vertex:

$$
\boxed{\mathcal M=\lambda+O(\lambda^2),\qquad |\mathcal M|^2=\lambda^2+O(\lambda^3).}
$$

There is no exchange graph at this order because there is no three-field interaction.

<a id="2/image-tree-level-contact-diagram-for-two-incoming-and-two-outgoing-real-scalar-particles"></a>
![](../../../../../past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-43-scalar-contact.png)

**[Figure 1](#2/image-tree-level-contact-diagram-for-two-incoming-and-two-outgoing-real-scalar-particles). Tree-level contact diagram for two incoming and two outgoing real scalar particles**.

For the [elastic scattering from a quartic scalar contact interaction](../../../../../elastic-scattering-from-a-quartic-scalar-contact-interaction.md), write $\sqrt s$ for the total centre-of-mass energy and $E_p=\sqrt s/2$ for the energy of each incoming particle. The incoming and outgoing spatial momentum magnitudes both equal $k=\sqrt{E_p^2-m^2}$, with $E_p>m$. The invariant incident flux is

$$
F=4\sqrt{(p_1\cdot p_2)^2-m^4}=8E_pk=4k\sqrt s.
$$

The [Lorentz-invariant phase-space measure](../../../../../lorentz-invariant-phase-space-measure.md) for two outgoing particles is

$$
d\Phi_2=(2\pi)^4\delta^4(p_1+p_2-p_3-p_4)\prod_{j=3}^4\frac{d^3p_j}{(2\pi)^3\,2E_j}.
$$

In the centre-of-mass frame, the spatial delta function sets $\mathbf p_4=-\mathbf p_3$, while the energy delta function has radial derivative $2k/E_p$. Therefore the [relativistic two-body phase space](../../../../../relativistic-two-body-phase-space.md) satisfies

$$
\frac{d\Phi_2}{d\Omega}=\frac{k}{16\pi^2\sqrt s}.
$$

The two outgoing real-scalar particles are identical. Integrating over the full solid angle counts each unordered pair twice, so include the [identical final-state symmetry factor](../../../../../identical-particle-factor-in-a-final-state-phase-space-integral.md) $1/2!$. This gives

$$
\boxed{\frac{d\sigma_{\rm event}}{d\Omega}=\frac1{2!}\frac{|\mathcal M|^2}{64\pi^2s}=\frac{\lambda^2}{128\pi^2s}+O(\lambda^3).}
$$

This is isotropic. When $E$ denotes each particle's energy, $s=4E^2$ and the full-sphere event density is **$\lambda^2/(512\pi^2E^2)$**. If $E$ denotes the total energy of the pair, $s=E^2$ and it is **$\lambda^2/(128\pi^2E^2)$**. Stating the answer in $s$ removes that energy-label ambiguity.

An equally valid angular convention selects one outgoing particle in a hemisphere, so each event is represented once. In that convention omit $1/2!$ and use $d\sigma/d\Omega=\lambda^2/(64\pi^2s)$ on the hemisphere, or $\lambda^2/(256\pi^2E_p^2)$. Both conventions give $\sigma_{\rm event}=\lambda^2/(32\pi s)$ at this order. The identical-state factor concerns counting final states and is separate from the vertex factorial.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 43](../../paper-43-split.md)
3. [Iii](../../split.md)
4. [2015](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
