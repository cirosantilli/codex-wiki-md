# Elliptical polarization

↑ **Parent:** [Polarization (waves)](polarization-waves.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Elliptical_polarization)

For an [elliptically polarized wave](elliptical-polarization.md), the tip of its transverse [vector](vector.md) traces an [ellipse](ellipse.md) at a fixed point during each [wave period](wave-period.md). For [polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md), this is the [electric field](electric-field.md) [vector](vector.md). With the real components in [polarization of waves](polarization-waves.md), assume $A_x,A_y>0$ and $\sin\delta\neq0$. Eliminating time gives

$$
\frac{E_x^2}{A_x^2}+\frac{E_y^2}{A_y^2}-\frac{2E_xE_y}{A_xA_y}\cos\delta=\sin^2\delta.
$$

A short derivation uses $\phi=\omega t$ and the [cosine](cosine.md) addition formula to obtain $E_y/A_y=(E_x/A_x)\cos\delta-\sin\phi\sin\delta$; squaring and using the [sine](sine.md) and [cosine](cosine.md) identity $\sin^2\phi=1-\cos^2\phi$ gives the displayed equation. Outside [phase quadrature](phase-quadrature.md), the mixed term gives a tilted [ellipse](ellipse.md); $A_x,A_y$ are component [wave amplitudes](wave-amplitude.md) and need not be its [semi-major and semi-minor axes](semi-major-and-semi-minor-axes.md).

In [phase quadrature](phase-quadrature.md), $\delta=\pm\pi/2$, the mixed term vanishes. For $(A_x,A_y)=(2,1)\,\mathrm{V/m}$, the [ellipse](ellipse.md) is $E_x^2/4+E_y^2=1$, its [semi-major and semi-minor axes](semi-major-and-semi-minor-axes.md) have lengths $2$ and $1\,\mathrm{V/m}$, and its [electric field](electric-field.md) magnitude varies between $1$ and $2\,\mathrm{V/m}$. At $\phi=\pi/4$ with $\delta=\pi/2$, the [electric field](electric-field.md) is $(\sqrt2,-1/\sqrt2)\,\mathrm{V/m}$ and has magnitude $\sqrt{5/2}\,\mathrm{V/m}$. Equal [wave amplitudes](wave-amplitude.md) instead give [circular polarization](circular-polarization.md), a special case of [elliptical polarization](elliptical-polarization.md) with constant magnitude. As $\delta$ approaches $0$ or $\pi$, the [ellipse](ellipse.md) collapses to a [line segment](line-segment.md) and gives [linear polarization](linear-polarization.md); this limit is degenerate rather than a nondegenerate [ellipse](ellipse.md).

Changing $\delta$ from $\pi/2$ to $-\pi/2$ reverses traversal of the same [ellipse](ellipse.md). In the displayed $x,y$ plot, $\delta=\pi/2$ moves from $(A_x,0)$ toward negative $y$ as time increases. A label such as right- or left-handed [circular polarization](circular-polarization.md) additionally requires a stated viewing direction and naming convention: viewing along propagation and viewing against propagation reverse the apparent rotation. [Feynman Lectures, I §33–1: polarization conventions](https://www.feynmanlectures.caltech.edu/I_33.html#Ch33-S1).

The [ellipse](ellipse.md) records both the relative [wave amplitudes](wave-amplitude.md) and the [phase difference](phase-difference.md) of two transverse [oscillations](oscillation.md). This separates a change of [polarization of waves](polarization-waves.md) from a change of overall [wave amplitude](wave-amplitude.md): multiplying both components by the same positive factor enlarges the [ellipse](ellipse.md) while preserving its shape and orientation.

A rotating ideal linear [polarizer](polarizer.md) can probe this geometry. For the $2:1$ [ellipse](ellipse.md) in [phase quadrature](phase-quadrature.md), [orthogonal projection](orthogonal-projection.md) onto a pass axis at [angle](angle.md) $\theta$ gives $E_{\mathrm{out}}(t)=2\cos\theta\cos\omega t-\sin\theta\sin\omega t$, in $\mathrm{V/m}$. Averaging its square over a [wave period](wave-period.md) gives $(4\cos^2\theta+\sin^2\theta)/2$, while the incoming squared [electric field](electric-field.md) magnitude averages to $5/2$. Thus the transmitted fraction of [light intensity](light-intensity.md) is $(4\cos^2\theta+\sin^2\theta)/5$: it is $4/5$ at $0^\circ$, $1/2$ at $45^\circ$ and $1/5$ at $90^\circ$. There is no single incident line of [linear polarization](linear-polarization.md) to insert into [Malus's law](malus-s-law.md); projecting the [electric field](electric-field.md) and averaging its square is the appropriate generalization. This measurement cannot distinguish $\delta=\pi/2$ from $\delta=-\pi/2$, because reversing the traversal leaves all these squared averages unchanged.

## ↑ Ancestors (4)

1. [Polarization (waves)](polarization-waves.md)
2. [Wave](wave.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Elliptical polarization](elliptical-polarization.md)
- [Polarization (waves)](polarization-waves.md)
- [Quarter-wave plate](quarter-wave-plate.md)
