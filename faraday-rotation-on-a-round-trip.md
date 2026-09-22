# Faraday rotation on a round trip

↑ **Parent:** [Faraday effect](faraday-effect.md)

[Faraday rotation](faraday-effect.md) exhibits [optical nonreciprocity](optical-nonreciprocity.md): with the bias [magnetic field](magnetic-field-split.md) held fixed, a retracing beam gains another rotation in the same laboratory sense. Natural [optical activity](optical-activity.md) in a reciprocal medium instead unwinds on retracing the path.[RP Photonics Encyclopedia, Faraday Effect, Rüdiger Paschotta: What is the Faraday Effect?, doubled rotation on a round trip](rp-photonics-encyclopedia-by-rudiger-paschotta/faraday-effect.md)

To reconcile this with the signed $B_\parallel$ formula, retain the laboratory $x,y,z$ axes for comparing physical lines. For the backward ray choose a right-handed ray basis $x'=x$, $y'=-y$, $z'=-z$. Its [magnetic flux density](magnetic-field-split.md) component is $B_\parallel'=-B_z$, so its local rotation increment is $-\theta$. But positive $y'$ is negative laboratory $y$: the backward increment is therefore $+\theta$ in the laboratory orientation plot. Reversing the ray reverses both the longitudinal component and the basis used for its signed [angle](angle.md). Reversing only one creates the false prediction of cancellation.

In fixed laboratory transverse components, define the [rotation matrix](rotation-matrix.md)

$$
R(\theta)=\begin{pmatrix}\cos\theta&-\sin\theta\\\sin\theta&\cos\theta\end{pmatrix}.
$$

For an ideal mirror at [normal incidence](normal-incidence.md) that contributes the same [complex amplitude](complex-amplitude.md) factor $r$ to both transverse components, the round-trip map is $rR(\theta)R(\theta)=rR(2\theta)$. The common mirror factor does not change the oscillation line. A reciprocal natural rotator instead gives $rR(-\alpha)R(\alpha)=rI$. This comparison assumes a retraced straight path and no additional polarization-changing elements.

For example, a chosen single-pass $30^\circ$ [Faraday rotation](faraday-effect.md) produces a returned line at $60^\circ$ to the original laboratory $x$ axis. A chosen reciprocal $30^\circ$ natural rotator returns it to $0^\circ$. The same addition makes an ideal [optical isolator](optical-isolator.md) possible: [polarizers](polarizer.md) at $0^\circ$ and $45^\circ$ surround a $45^\circ$ Faraday rotator. Forward [light](light.md) follows $0^\circ\to45^\circ$ and passes. Returning [light](light.md) selected at $45^\circ$ reaches $90^\circ$ at the entrance [polarizer](polarizer.md) and is rejected by [Malus's law](malus-s-law.md). Real transmission loss and incomplete extinction limit the isolation.

## ↑ Ancestors (8)

1. [Faraday effect](faraday-effect.md)
2. [Polarization of an electromagnetic wave](polarization-of-an-electromagnetic-wave.md)
3. [Plane electromagnetic wave](plane-electromagnetic-wave.md)
4. [Electromagnetic wave](electromagnetic-wave-split.md)
5. [Electromagnetism](electromagnetism-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Faraday effect](faraday-effect.md)
- [Optical isolator](optical-isolator.md)
- [Optical nonreciprocity](optical-nonreciprocity.md)
