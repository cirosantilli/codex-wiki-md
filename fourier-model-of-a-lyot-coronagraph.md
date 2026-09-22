# Fourier model of a Lyot coronagraph

↑ **Parent:** [Lyot coronagraph](lyot-coronagraph.md)

Consider an ideal coherent [monochromatic wave](monochromatic-wave.md) from an unresolved source on the [optical axis](optical-axis.md), a uniform circular [entrance pupil](entrance-pupil.md) of [diameter](diameter.md) $D$, and ideal relay optics without [wavefront errors](wavefront-error.md). In the scalar [Fraunhofer diffraction](fraunhofer-diffraction.md) approximation, a [Fourier transform](fourier-transform-split.md) carries the pupil's [complex amplitude](complex-amplitude.md) into the image plane. Choose dimensionless pupil coordinates $\mathbf x$ in units of $D$ and angular coordinates $\mathbf u=D\boldsymbol\theta/\lambda$, where $\lambda$ is the [wavelength](wavelength.md). Define

$$
P(\mathbf x)=\begin{cases}1,&|\mathbf x|\leq1/2,\\0,&|\mathbf x|>1/2,\end{cases}
\qquad A=\mathcal F P,\qquad
(\mathcal F P)(\mathbf u)=\int_{\mathbb R^2}P(\mathbf x)e^{-2\pi i\mathbf x\cdot\mathbf u}\,d^2\mathbf x.
$$

The [coronagraphic focal plane mask](coronagraphic-focal-plane-mask.md) has transmission $M=1-W$, with $W=1$ inside the occulting disk and $W=0$ outside. Thus the field immediately after the mask is $MA$. Outside the disk $M=1$, so the local [wave intensity](intensity-physics.md) is still $|A|^2$: hiding the core has left those rings intact. Reimaging an unlimited pupil gives

$$
E_{\rm L}=\mathcal F^{-1}(MA)=P-P*\mathcal F^{-1}W,
\qquad
A_{\rm final}=\mathcal F(LE_{\rm L}),
\qquad I_{\rm final}=|A_{\rm final}|^2,
$$

where $*$ is [convolution](convolution.md), $L$ is the [Lyot stop](lyot-stop.md) transmission, and the proportionality constant in the [irradiance](irradiance.md) is omitted. Coordinate reversals from physical relay optics are absorbed into the coordinate choice. These equations use [wave amplitudes](wave-amplitude.md) throughout propagation; applying a [Fourier transform](fourier-transform-split.md) to [wave intensity](intensity-physics.md) would give a different and incorrect model. This is the pupil/image calculation described by Sivaramakrishnan et al.; the circular disk and numerical choices below are our illustrative specialization. [Sivaramakrishnan et al., 2001, §2.1, equations 2–6](https://ao.jpl.nasa.gov/Publications/Technical/2001ApJ.sivaramakrishnan.AO.pdf).

The subtraction explains the beauty of the arrangement: in much of the interior, the original pupil field and the [convolution](convolution.md) term nearly cancel. Near a boundary, that cancellation is incomplete. The [Lyot stop](lyot-stop.md) can therefore block a region containing disproportionately much unwanted [light](light.md). A hard-edged [coronagraphic focal plane mask](coronagraphic-focal-plane-mask.md) has a transform with extended tails, so the interior need not be perfectly dark. With an unlimited relay, $L=1$ gives $A_{\rm final}=MA$ exactly: no further ring suppression occurs. A stop covering the full original [optical pupil](optical-pupil.md) instead uses $L=P$ and already clips field outside the [optical pupil](optical-pupil.md); an undersized [Lyot stop](lyot-stop.md) clips more of the remaining rim.

<a id="image-fourier-transform-model-of-a-circular-pupil-lyot-coronagraph"></a>
![](coronagraph-circular-pupil-fourier-toy.png)

**[Figure 16](#image-fourier-transform-model-of-a-circular-pupil-lyot-coronagraph). Fourier transform model of a circular-pupil Lyot coronagraph**. Original [Fourier transform](fourier-transform-split.md) calculation for a circular [entrance pupil](entrance-pupil.md): the residual [wave intensity](intensity-physics.md) before the [Lyot stop](lyot-stop.md), and final radial profiles with different pupil openings. All curves use the same unmasked stellar peak normalization. Ideal toy, not measured data.

The toy uses a [coronagraphic focal plane mask](coronagraphic-focal-plane-mask.md) of angular [radius](radius.md) $3\lambda/D$ and a [Lyot stop](lyot-stop.md) of [diameter](diameter.md) $0.8D$. The [discrete Fourier transform](discrete-fourier-transform-split.md) grid has $1024\times1024$ samples, with 128 across $D$ and angular sampling $0.125\lambda/D$; it approximates the continuous equations on a finite periodic domain. The plot averages [wave intensity](intensity-physics.md) in annuli of width $0.25\lambda/D$. Over the annulus $4\leq|\mathbf u|\leq10$, the mean [wave intensity](intensity-physics.md) divided by the direct stellar peak is approximately $1.40\times10^{-4}$ without a [coronagraph](coronagraph.md), the same with only the focal mask and an unlimited relay, $4.44\times10^{-5}$ with the mask and full pupil, and $1.66\times10^{-6}$ with the mask and $0.8D$ [Lyot stop](lyot-stop.md). Thus the undersized opening reduces this particular annular mean about 27-fold relative to the full-pupil comparison. It does not suppress every direction by that factor, and these values do not predict a real instrument's detection limit.

The ideal toy excludes a central obstruction, support vanes, [scattering of light](scattering-of-light.md), [wavefront errors](wavefront-error.md), atmospheric effects, a spread of [wavelengths](wavelength.md), pointing drift and detector noise. It also contains only the star: no simulated planet or [solar corona](solar-corona.md). For a far off-axis source whose image misses the [coronagraphic focal plane mask](coronagraphic-focal-plane-mask.md), the continuous geometric [coronagraph throughput](coronagraph-throughput.md) of the $0.8D$ opening tends to $0.8^2=0.64$ relative to the full disk. Rejecting stellar [light](light.md) therefore costs some desired [light](light.md) as well. Enlarging the [coronagraphic focal plane mask](coronagraphic-focal-plane-mask.md) narrows the characteristic scale of its pupil-plane transform by the [scaling property of the Fourier transform](scaling-property-of-the-fourier-transform.md), but also hides a larger neighborhood of the source.

## ↑ Ancestors (6)

1. [Lyot coronagraph](lyot-coronagraph.md)
2. [Coronagraph](coronagraph.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Diffraction-limited system](diffraction-limited-system.md)
