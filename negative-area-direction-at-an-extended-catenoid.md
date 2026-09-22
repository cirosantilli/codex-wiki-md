# Negative area direction at an extended catenoid

↑ **Parent:** [Axisymmetric second variation of a catenoid](axisymmetric-second-variation-of-a-catenoid.md)

A [catenoid](catenoid.md) has zero [mean curvature](mean-curvature.md), but need not minimize area for its fixed boundary rings. For the profile $y(x)=\cosh x$ on $[-2,2]$, take an endpoint-zero variation $\eta(x)=\cosh x-\cosh2$. The [second variation](second-variation.md) of the rotational area is

$$
\delta^2J[\eta]=2\pi\int_{-2}^2\operatorname{sech}^2x\,(\eta'^2-\eta^2)\,dx
=2\pi\{4C\arctan(\sinh2)-2(1+C^2)\tanh2\},\qquad C=\cosh2.
$$

To derive the integral, differentiate $y\sqrt{1+y'^2}$ twice, then integrate its mixed term by parts; the endpoint term vanishes. To evaluate it, substitute $\eta'^2-\eta^2=-1-C^2+2C\cosh x$, using the antiderivatives of $\operatorname{sech}x$ and $\operatorname{sech}^2x$. The result is negative because $\arctan(\sinh2)<\pi/2$ and $(C+C^{-1})\tanh2>\pi$.

Small positive and negative perturbations remain positive and preserve the boundary values. The first variation vanishes, while the negative second variation gives nearby smaller areas. Thus being a [minimal surface](minimal-surface.md) in the zero-mean-curvature sense is a stationarity condition, not a guarantee of area minimization for arbitrary boundary separations.

## ↑ Ancestors (9)

1. [Axisymmetric second variation of a catenoid](axisymmetric-second-variation-of-a-catenoid.md)
2. [Catenoid is a minimal surface](catenoid-is-a-minimal-surface.md)
3. [Catenoid](catenoid.md)
4. [Surface of revolution](surface-of-revolution.md)
5. [Differential geometry](differential-geometry-split.md)
6. [Geometry and topology](geometry-and-topology-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)
