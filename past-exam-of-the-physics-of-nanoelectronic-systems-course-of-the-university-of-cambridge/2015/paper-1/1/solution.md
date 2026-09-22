<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

**A trajectory-resolving ballistic experiment.** Use a high-mobility modulation-doped GaAs-AlGaAs heterostructure with a [two-dimensional electron gas](../../../../two-dimensional-electron-gas.md). Grow the layers by molecular-beam epitaxy, separate the donor layer from the conducting interface with an undoped spacer, and pattern an isolated mesa with ohmic reservoir contacts. Electron-beam lithography defines metal [split gates](../../../../split-gate.md); negative gate [voltage](../../../../voltage.md) depletes the underlying [electron](../../../../electron.md) gas, leaving narrow adjustable injector and collector [quantum point contacts](../../../../quantum-point-contact.md) along an edge. Keep the relevant path shorter than the momentum-relaxation [mean free path](../../../../mean-free-path.md), cool to suppress [phonon scattering](../../../../phonon-scattering.md) and thermal smearing, and use a small excitation to avoid heating.

Inject a low-frequency current through one contact to a distant drain and measure the collector's open-circuit [voltage](../../../../voltage.md) with a high-input-impedance amplifier. Sweep perpendicular [magnetic field](../../../../magnetic-field-split.md) and gate settings. The [cyclotron radius](../../../../cyclotron-radius.md) is $r_c=\hbar k_F/(e|B|)$, with $k_F=\sqrt{2\pi n_s}$ for a spin-degenerate single-valley gas. For contact separation $L$, semicircular or skipping trajectories focus into the collector when

$$
\boxed{L=2jr_c,\qquad |B_j|=\frac{2j\hbar k_F}{eL},\quad j=1,2,\ldots.}
$$

The appropriate field sign bends carriers toward the collector; the opposite sign suppresses the peaks. Density-dependent focusing positions, suppression with increased scattering and reproducible gate control distinguish directional ballistic propagation from an ordinary diffusive [voltage](../../../../voltage.md). [Quantum interference](../../../../quantum-interference.md) may add fine structure, but the basic focusing signal does not require phase coherence over every path. Split-gate injection and collection in a two-dimensional gas were directly demonstrated in the original focusing experiment.[1989 primary publication, institutional abstract: split Schottky gates, injector/collector, skipping orbits and field-dependent focusing](../../../../coherent-electron-focusing-with-quantum-point-contacts-in-a-two-dimensional-electron-gas-by-h-van-houten-and-others.md)

**Multi-probe current bookkeeping.** For one directed spin-resolved [mode](../../../../mode-statistics.md), velocity times one-dimensional [density of states](../../../../density-of-states.md) gives a particle flux $dE/h$. A small reservoir electrochemical-energy shift $\mu_j$ therefore supplies excess flux $\mu_j/h$. Let $N_i$ be the number of propagating [modes](../../../../mode-statistics.md) at lead $i$, $R_{ii}$ their summed return probability, and $T_{ij}$ the total transmission from reservoir $j$ into lead $i$. Multiplying outgoing-minus-incoming [electron](../../../../electron.md) flux by charge $-e$ gives the source's convention,

$$
\boxed{I_i=-\frac eh(N_i-R_{ii})\mu_i
+\frac eh\sum_{j\ne i}T_{ij}\mu_j.}
$$

The reservoirs equilibrate arriving carriers; an ideal [voltage](../../../../voltage.md) probe adjusts its [chemical potential](../../../../chemical-potential-split.md) until its net current vanishes. Here $\mu_i$ is an energy, not a [voltage](../../../../voltage.md). Choose the lead-voltage convention $\mu_i=-eV_i$ and positive [conventional current](../../../../conventional-current.md) injected into the junction. The working equation is then

$$
\boxed{I_i=g_0\left[(N_i-R_{ii})V_i-\sum_{j\ne i}T_{ij}V_j\right],\qquad g_0=e^2/h.}
$$

Conservation of scattering probability and [gauge invariance](../../../../gauge-invariance.md) require both column and row balance: every outgoing channel is accounted for and equal [voltages](../../../../voltage.md) give zero current. The counts $M,N$ below include every occupied internal channel; an extra factor of two must not be inserted if [spin](../../../../spin.md) is already counted. If one instead counts orbital channels with unresolved [spin degeneracy](../../../../spin-degeneracy.md), double all transmission counts consistently.

**Zero-field routing.** The original diagram labels lead 1 at the left, 2 above, 3 at the right and 4 below. With columns denoting injectors and rows collectors, straight-through ballistic routing and the stipulated excess-wide-channel rule give

$$
\mathsf T_0=\begin{pmatrix}
0&0&M&0\\
0&0&0&M\\
M&0&0&N-M\\
0&M&N-M&0
\end{pmatrix},\qquad (N_1,N_2,N_3,N_4)=(M,M,N,N).
$$

There is no reflection in this ideal routing model. Set $V_4=0$, $I_2=I_3=0$, and $I_1=I=-I_4$. The two probe equations give

$$
V_2=0,\qquad V_3=\frac MN V_1,
\qquad I=g_0M\left(1-\frac MN\right)V_1.
$$

Thus

$$
\boxed{R_{14,23}(0)=\frac{V_2-V_3}{I}=-\frac{h}{e^2(N-M)}.}
$$

The derivation assumes $N>M>0$. At $N=M$, the ideal network splits into two disconnected opposite-lead pairs and cannot carry the imposed 1-to-4 current at finite [voltage](../../../../voltage.md); the divergence diagnoses failure of that limiting transport configuration, not an infinite dissipative resistance of each channel. Negative [bend resistance](../../../../bend-resistance.md) is a nonlocal [voltage](../../../../voltage.md) sign, compatible with positive total dissipated power.

**Positive field.** At $+B_0$, left-deflected incoming carriers go $1\to2$, $2\to3$, $3\to4$. Lead 4 supplies $M$ [modes](../../../../mode-statistics.md) to narrow lead 1; the remaining $N-M$ enter wide lead 3. The balanced transmission matrix is

$$
\mathsf T_+=\begin{pmatrix}
0&0&0&M\\
M&0&0&0\\
0&M&0&N-M\\
0&0&N&0
\end{pmatrix}.
$$

Therefore $V_2=V_1$, $V_3=MV_1/N$ and $I=g_0MV_1$, giving

$$
\boxed{R_{14,23}(+B_0)=\frac h{e^2}\frac{N-M}{MN}
=\frac h{e^2}\left(\frac1M-\frac1N\right)>0.}
$$

**Negative field.** Reversing the chirality gives $\mathsf T_-=\mathsf T_+^{\mathsf T}$, as expected from reciprocity for this spin-independent routing model. With $V_4=0$, the zero-current conditions become $V_3=V_4=0$ and $V_2=V_3=0$. Thus

$$
\boxed{R_{14,23}(-B_0)=0.}
$$

This does not contradict reciprocity: the general relation interchanges the current and [voltage](../../../../voltage.md) lead pairs when reversing field; it does not require the same fixed-contact four-terminal resistance to be even in $B$.

<a id="1/image-original-transmission-matrix-bookkeeping-for-the-three-ideal-field-limits-rows-collect-modes-injected-by-columns"></a>
![](../../../../past-exam-of-the-physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge/2015/paper-1-bend-routing.png)

**[Figure 1](#1/image-original-transmission-matrix-bookkeeping-for-the-three-ideal-field-limits-rows-collect-modes-injected-by-columns). Original transmission-matrix bookkeeping for the three ideal field limits; rows collect modes injected by columns**.

**Comparison with the measured trace.** The PDF shows a negative region around zero field, approximately zero signal at sufficiently negative field, and a positive rising resistance near $+0.4\ {\rm T}$ and above. These signs match the three routing limits. Near zero field the depth is roughly a few tenths of a kilohm; the graph does not supply $M,N$, so there is no justified exact amplitude fit. Rounded corners, collimation and finite [cyclotron radius](../../../../cyclotron-radius.md) continuously change which outgoing lead is reached between the ideal limits. Skipping trajectories and geometrical focusing can produce shoulders or resonances. At larger positive fields magnetic depopulation and [spin](../../../../spin.md) resolution can change the [mode](../../../../mode-statistics.md) counts, increasing the positive resistance or producing structure; disorder, incomplete equilibration and finite temperature round ideal features. These are candidate mechanisms, not uniquely established assignments of every small feature from one trace.

## ↑ Ancestors (13)

1. [1](../1.md)
2. [Paper 1](../../paper-1-split.md)
3. [2015](../../split.md)
4. [Past exam of the physics of Nanoelectronic Systems course of the University of Cambridge](../../../split.md)
5. [Physics of Nanoelectronic Systems course of the University of Cambridge](../../../../physics-of-nanoelectronic-systems-course-of-the-university-of-cambridge.md)
6. [Physics course of the year 4 of the natural sciences course of the University of Cambridge](../../../../physics-course-of-the-year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 4 of the natural sciences course of the University of Cambridge](../../../../year-4-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../list-of-universities.md)
13. [Codex Wiki](../../../../split.md)
