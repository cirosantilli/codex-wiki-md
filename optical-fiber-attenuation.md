# Optical fiber attenuation

↑ **Parent:** [Optical fiber](optical-fiber.md)

[Optical fiber attenuation](optical-fiber-attenuation.md) is the reduction of transmitted [optical power](optical-power.md) along an [optical fiber](optical-fiber.md). Define a positive loss in [decibels](decibel.md) by comparing [optical power](optical-power.md) $P(0)$ already launched into the guide with surviving [optical power](optical-power.md) $P(z)$:

$$
A(z)=10\log_{10}\!\left(\frac{P(0)}{P(z)}\right)\,\mathrm{dB}.
$$

The factor ten applies to a [power](power.md) ratio; the factor twenty applies to a [wave amplitude](wave-amplitude.md) ratio only when [power](power.md) is proportional to its square under the same conditions.[Introduction to Optical Fibers, dB, Attenuation and Measurements, What is a Decibel?, Base 10 Logarithm Rules and Power/Voltage Gains: attenuation convention](introduction-to-optical-fibers-db-attenuation-and-measurements-by-cisco.md)

For a uniform illustrative model with constant loss coefficient $\alpha_{\rm dB}$ in $\mathrm{dB/km}$ and distance $z$ in kilometres,

$$
A(z)=\alpha_{\rm dB}z,\qquad
\frac{P(z)}{P(0)}=10^{-A(z)/(10\,\mathrm{dB})}.
$$

For $\alpha_{\rm dB}=0.2\,\mathrm{dB/km}$ over $10\,\mathrm{km}$, the loss is $2\,\mathrm{dB}$ and

$$
\frac{P(10\,\mathrm{km})}{P(0)}=10^{-0.2}\simeq0.630957.
$$

Thus about $63.1\%$ of the launched [optical power](optical-power.md) survives and $36.9\%$ is lost. This is an illustrative coefficient, not a property of all [optical fibers](optical-fiber.md), and is independent of the earlier illustrative [refractive indices](refractive-index.md).

<a id="image-equal-distance-increments-add-decibel-loss-and-multiply-surviving-power"></a>
![](optical-fiber-distance-and-power-loss.png)

**[Figure 12](#image-equal-distance-increments-add-decibel-loss-and-multiply-surviving-power). Equal distance increments add decibel loss and multiply surviving power**.

The [exponential decay](exponential-decay.md) follows from assuming each equal distance interval transmits the same fraction. For two such intervals, [power](power.md) ratios multiply; their [logarithms](logarithm.md) add, so the losses in [decibels](decibel.md) add. Two $5\,\mathrm{km}$ sections each transmit $10^{-0.1}\simeq0.794328$; together they transmit $(0.794328)^2\simeq0.630957$. The loss curve is straight in [decibels](decibel.md) and curved on a linear [power](power.md) scale.

[Wave absorption](wave-absorption.md) and [scattering of light](scattering-of-light.md) can remove guided [optical power](optical-power.md) even in a straight fibre, while bends can let it escape. Entrance losses, joints and connectors contribute additional losses; they belong separately from a uniform distance coefficient. This is why a measured end-to-end [power](power.md) ratio need not equal the straight-fibre model.[Introduction to Optical Fibers, dB, Attenuation and Measurements, Understand Insertion Loss and Calculate a Power Budget: joint losses, launch dependence and distance contribution](introduction-to-optical-fibers-db-attenuation-and-measurements-by-cisco.md)

**Table of contents**

- [Optical fiber cutback measurement](optical-fiber-cutback-measurement.md)

## ↑ Ancestors (6)

1. [Optical fiber](optical-fiber.md)
2. [Optical instrument](optical-instrument-split.md)
3. [Optics](optics-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Optical fiber](optical-fiber.md)
- [Optical fiber attenuation](optical-fiber-attenuation.md)
- [Optical fiber cutback measurement](optical-fiber-cutback-measurement.md)
- [Optical fiber purity and low-loss transmission](optical-fiber-purity-and-low-loss-transmission.md)
