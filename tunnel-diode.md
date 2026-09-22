# Tunnel diode

↑ **Parent:** [P-n junction](p-n-junction.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Tunnel_diode)

A [tunnel diode](tunnel-diode.md) is a [p-n junction](p-n-junction.md) with sufficiently heavy [semiconductor doping](semiconductor-doping.md) on both sides to make a thin [depletion region](depletion-region.md) and permit substantial [interband tunnelling](interband-tunnelling.md). The neutral regions are [degenerate semiconductors](degenerate-semiconductor.md). Its distinctive forward [current-voltage characteristic](current-voltage-characteristic.md) contains a peak followed by a valley: over part of the curve, increasing the applied [electric potential difference](electric-potential-difference.md) decreases the [electric current](electric-current.md). The [Esaki tunnel-diode experiment](esaki-tunnel-diode-experiment.md) made this behavior experimentally concrete.

The useful quantity is the local slope, not the ratio of total voltage to total [electric current](electric-current.md). With conventional [electric current](electric-current.md) $I$ entering the positive-voltage terminal, define

$$
g_d=\frac{dI}{dV},\qquad r_d=\frac{dV}{dI}=\frac1{g_d}\quad(g_d\ne0).
$$

[Negative differential resistance](negative-differential-resistance.md) means $g_d<0$, hence $r_d<0$ where defined. A forward [operating point](operating-point.md) can still have $V>0$, $I>0$ and absorbed [power](power.md) $VI>0$. A small voltage increase then gives a negative current increment; this does not make the total [electric current](electric-current.md) negative or turn the device into an unlimited source of [energy](energy-split.md). The external supply sets the [operating point](operating-point.md) and supplies the [energy](energy-split.md) available for an [electronic amplifier](electronic-amplifier.md).

An original idealized construction explains the shape. Put the [n-type semiconductor](n-type-semiconductor.md) on the left and the [p-type semiconductor](p-type-semiconductor.md) on the right. Take $q>0$ as the [elementary charge](elementary-charge.md) and $V=V_p-V_n$. Increasing [forward bias](forward-bias.md) lowers the right-hand [electron](electron.md) [energy](energy-split.md) levels relative to the left. Denote the two reservoir [electrochemical potentials](electrochemical-potential.md) by $\mu_n,\mu_p$, so that $\mu_n-\mu_p=qV$. At zero [temperature](temperature-split.md), occupied left-hand [conduction band](conduction-band.md) states extend up to $\mu_n$; empty right-hand [valence band](valence-band.md) states start at $\mu_p$. For transfer conserving [electron](electron.md) [energy](energy-split.md), the available interval is

$$
\max(E_{c,n},\mu_p)<E<\min(\mu_n,E_{v,p}).
$$

It is nonempty only when its upper endpoint exceeds its lower endpoint. Both an occupied initial [quantum state](quantum-state.md) and an empty final [quantum state](quantum-state.md) must exist at the same [energy](energy-split.md). The [Pauli exclusion principle](pauli-exclusion-principle.md) prevents transfer into an already occupied final [quantum state](quantum-state.md).

For the original diagram, choose arbitrary [energy](energy-split.md) units with $E_{c,n}=-0.5$, $\mu_n=0$, $\mu_p=-u$ and $E_{v,p}=0.5-u$, where $u$ is $qV$ in those units. The available interval has width

$$
L(u)=\max\!\left(0,\min(0,0.5-u)-\max(-0.5,-u)\right),\qquad u\ge0.
$$

Thus $L(0.25)=0.25$, $L(0.50)=0.50$, $L(0.70)=0.30$, and $L(1.15)=0$. Initially [forward bias](forward-bias.md) opens a transfer window; further [forward bias](forward-bias.md) closes it by moving the right-hand [valence band](valence-band.md) edge below the left-hand [conduction band](conduction-band.md) edge. This is a state-counting illustration, not a formula for a measured [electric current](electric-current.md).

<a id="image-tunnel-diode-energy-band-alignment-and-occupied-to-empty-state-overlap"></a>
![](tunnel-diode-band-state-overlap.png)

**[Figure 1](#image-tunnel-diode-energy-band-alignment-and-occupied-to-empty-state-overlap). Tunnel diode: energy band alignment and occupied-to-empty state overlap**. [Source](tunnel-diode-band-state-overlap.py). Original chosen [energy band](energy-band.md) construction, with [n-type semiconductor](n-type-semiconductor.md) on the left and [p-type semiconductor](p-type-semiconductor.md) on the right. Blue shading denotes occupied reservoir states; orange hatching denotes empty reservoir states. Green arrows mark equal-[energy](energy-split.md) transfer. The central barrier and [band bending](band-bending.md) are schematic; all [energies](energy-split.md) are arbitrary, and the drawing is not an experimental image or measured band profile.

For [reverse bias](reverse-bias.md), the transfer direction changes: occupied right-hand [valence band](valence-band.md) states can feed empty left-hand [conduction band](conduction-band.md) states. In the same construction, $u=-0.70$ opens the interval $0<E<0.70$ for this reverse transfer. A narrow [depletion region](depletion-region.md) allows a large reverse [quantum tunnelling](quantum-tunnelling.md) [electric current](electric-current.md) at small [electric potential difference](electric-potential-difference.md), whereas the ordinary [Shockley diode equation](shockley-diode-equation.md) predicts only a small reverse saturation [electric current](electric-current.md) before [diode reverse breakdown](diode-reverse-breakdown.md). At zero [biasing](biasing.md), equal reservoir occupations give zero net [electric current](electric-current.md); [quantum tunnelling](quantum-tunnelling.md) does not require a net equilibrium flow.

A finite-[temperature](temperature-split.md) refinement replaces sharp occupation cutoffs with the [Fermi-Dirac distribution](fermi-dirac-distribution.md). An illustrative weak-transfer expression is

$$
I_{n\to p}(V)=K\int \mathcal W(E,V)\,[f_n(E)-f_p(E)]\,dE,\qquad K>0.
$$

Here $\mathcal W\ge0$ describes allowed initial/final [quantum states](quantum-state.md) and their coupling, and $f_n,f_p$ are [Fermi-Dirac distributions](fermi-dirac-distribution.md) with the respective [electrochemical potentials](electrochemical-potential.md). The occupation difference follows by subtracting the reverse transfer factor from the forward one: $f_n(1-f_p)-f_p(1-f_n)=f_n-f_p$. An overlap interval alone does not determine $\mathcal W$: [transmission probability](transmission-probability.md), [density of states](density-of-states.md), [crystal momentum](crystal-momentum.md) selection and [phonons](phonon.md) can matter. A complete [germanium](germanium.md) calculation is more demanding than multiplying two constant [density of states](density-of-states.md) factors. At larger [forward bias](forward-bias.md), ordinary [carrier injection](carrier-injection.md) and [diffusion](diffusion.md) supply a rising current branch even after direct band overlap is lost.

**Table of contents**

- [Esaki tunnel-diode experiment](esaki-tunnel-diode-experiment.md)
- [Tunnel-diode load-line stability](tunnel-diode-load-line-stability.md)

## ↑ Ancestors (4)

1. [P-n junction](p-n-junction.md)
2. [Semiconductor](semiconductor-split.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Degenerate semiconductor](degenerate-semiconductor.md)
- [Depletion region](depletion-region.md)
- [Interband tunnelling](interband-tunnelling.md)
- [Josephson junction](josephson-junction.md)
- [Negative differential resistance](negative-differential-resistance.md)
- [P-n junction](p-n-junction.md)
- [Solution](past-exam-of-the-mphil-in-micro-and-nanotechnology-enterprise-course-of-the-university-of-cambridge/2022/paper-2/section-b/21/ii/e/solution.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2016/paper-1/section-c/c11/b/solution.md)
- [Tunnel diode](tunnel-diode.md)
- [Tunnel-diode load-line stability](tunnel-diode-load-line-stability.md)
