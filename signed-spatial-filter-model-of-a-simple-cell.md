# Signed spatial filter model of a simple cell

↑ **Parent:** [Simple cell](simple-cell.md)

A [signed spatial filter model of a simple cell](signed-spatial-filter-model-of-a-simple-cell.md) assigns a weight $K_{ij}$ to each sampled location and takes its [dot product](dot-product.md) with the [visual contrast](visual-contrast.md) image $C_{ij}$. Positive weights favor bright features; negative weights favor dark features. The signed drive

$$
D=\sum_{i,j}K_{ij}C_{ij},\qquad R=\max(0,D)
$$

is a [linear function](linear-function.md) of the image, while the [rectified linear unit](rectified-linear-unit.md) output $R$ is nonlinear. $D$ and $R$ below are arbitrary model units. To obtain a predicted firing rate one would need a calibrated gain, background response and possibly a different output function. The model does not generate a [spike train](spike-train.md); a [linear-nonlinear-Poisson cascade model](linear-nonlinear-poisson-cascade-model.md) adds a stochastic event-generation assumption.

For the first diagram, every one of five rows has weights

$$
(K_{i1},K_{i2},K_{i3},K_{i4},K_{i5})=(-1/20,-1/20,1/5,-1/20,-1/20).
$$

A bright central column, with $C_{i3}=1$ and zero elsewhere, gives $D=5/5=1$. A bright middle row gives $D=-1/20-1/20+1/5-1/20-1/20=0$; a uniformly bright patch also gives $D=0$, since every row sums to zero. Move the bright column one site right: $D=5(-1/20)=-1/4$, so $R=0$. Make that shifted column dark instead: $D=1/4$ and $R=1/4$. Thus an OFF-like weight can increase output for darkness. A negative weight is a descriptive sensitivity, not evidence for a particular inhibitory [synapse](synapse.md).

For a smooth example use the real, even [Gabor filter](gabor-filter.md)

$$
K(x,y)=\exp\!\left(-\frac{x^2}{2\sigma_x^2}-\frac{y^2}{2\sigma_y^2}\right)\cos(qx),\qquad C_{\theta,\varphi}(x,y)=\cos\!\bigl(q(x\sin\theta-y\cos\theta)+\varphi\bigr).
$$

The [Gaussian function](gaussian-function.md) localizes the weights; the [cosine](cosine.md) supplies alternating polarity. Choose $\sigma_x=1/2$, $\sigma_y=1$ and $q=\pi$ in arbitrary spatial units. The stripes' [spatial frequency](spatial-frequency.md) is $q/(2\pi)=1/2$ cycles per unit. Their axis makes [angle](angle.md) $\theta$ with horizontal, while brightness changes across the perpendicular axis. $\varphi$ is their spatial [phase](phase-waves.md). Normalize the full-plane [integral](integral.md) of $KC_{\theta,\varphi}$ by its value at $\theta=\pi/2$, $\varphi=0$. The [Gaussian integral](gaussian-integral.md) and the product identity for [cosines](cosine.md) give

$$
D(\theta,\varphi)=A(\theta)\cos\varphi,\qquad R(\theta,\varphi)=\max(0,D(\theta,\varphi)),
$$

where

$$
A(\theta)=\frac{\exp\!\left[-\frac{q^2}{2}\left(\sigma_x^2(\sin\theta-1)^2+\sigma_y^2\cos^2\theta\right)\right]+\exp\!\left[-\frac{q^2}{2}\left(\sigma_x^2(\sin\theta+1)^2+\sigma_y^2\cos^2\theta\right)\right]}{1+\exp(-2\sigma_x^2q^2)}.
$$

At $\varphi=0$, horizontal stripes give $R\approx0.004159$, $60^\circ$ stripes give $R\approx0.286741$, and vertical stripes give $R=1$. At the same vertical orientation, $\varphi=\pi/2$ gives $D=R=0$, while reversing the polarity with $\varphi=\pi$ gives $D=-1$ and $R=0$. The preferred axis persists while the response changes dramatically with position. Shifting the vertical stripes by a quarter of their wavelength changes [phase](phase-waves.md) by $\pi/2$ up to sign, without rotating them.

These are two different toy filters, not discretizations of the same fitted [receptive field](receptive-field.md). The discrete filter exactly rejects a uniform contrast patch; this [Gabor filter](gabor-filter.md) need not reject uniform contrast because its weight [integral](integral.md) need not vanish. Neither toy includes stimulus history, recurrent interactions, saturation or a measured response baseline. Their value is a transparent prediction: [orientation selectivity](orientation-selectivity.md) can emerge from spatial summation, and it does not by itself imply tolerance to [phase](phase-waves.md).

## ↑ Ancestors (5)

1. [Simple cell](simple-cell.md)
2. [Primary visual cortex](primary-visual-cortex.md)
3. [Neuroscience](neuroscience.md)
4. [Biology](biology-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Gabor filter](gabor-filter.md)
- [Orientation selectivity](orientation-selectivity.md)
- [Primary visual cortex](primary-visual-cortex.md)
- [Signed spatial filter model of a simple cell](signed-spatial-filter-model-of-a-simple-cell.md)
- [Simple cell](simple-cell.md)
