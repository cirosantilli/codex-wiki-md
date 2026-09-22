# Fizeau experiment path-length convention

↑ **Parent:** [Fizeau experiment](fizeau-experiment.md)

Use the schematic below to count the [water](water.md) traversals explicitly. Each stationary tube has laboratory length $\ell$. In the displayed setting, upper-tube [water](water.md) flows right and lower-tube [water](water.md) flows left, each at [speed](speed.md) $u>0$. Beam A goes right through the upper tube, exchanges tubes at the far optics, and returns left through the lower tube: it follows the flow twice. Beam B goes right through the lower tube and returns left through the upper tube: it opposes the flow twice. Each complete beam path therefore contains total [water](water.md) length $L=2\ell$, not $\ell$ or $4\ell$. The connecting air paths and fixed optics are assumed to contribute no flow-dependent [phase difference](phase-difference.md).

<a id="image-fizeau-counterflow-paths"></a>
![](fizeau-counterflow-paths.png)

**[Figure 8](#image-fizeau-counterflow-paths). Counterflow path accounting: beam A follows the water in both tubes, beam B opposes it, and each beam traverses total water length 2ℓ**. Original schematic of the tube exchange and recombination, not a scaled optical ray trace. Parallel coloured lines separate overlapping counterpropagating beams for readability. The grey arrows show [water](water.md) flow; reversing both grey arrows exchanges the roles of A and B.

Let $v_+$ and $v_-$ be positive [phase velocity](phase-velocity.md) magnitudes along and against the [water](water.md) flow:

$$
v_+=\frac{c/n+u}{1+u/(nc)},\qquad
v_-=\frac{c/n-u}{1-u/(nc)},\qquad
\Delta t=t_B-t_A=L\left(\frac1{v_-}-\frac1{v_+}\right).
$$

For a laboratory source of [frequency](frequency.md) $\nu=c/\lambda_0$, where $\lambda_0$ is its vacuum [wavelength](wavelength.md), define the signed [interference fringe](interference-fringe.md) offset $N$ by the propagation [phase difference](phase-difference.md) $\Delta\phi=2\pi\nu\Delta t=2\pi N$. This is an equivalent phase delay between steady beams; no stopwatch resolves their transit-time difference. Subtract the zero-flow baseline and expand to first order:

$$
\Delta t\simeq\frac{2Lu}{c^2}(n^2-1)=\frac{4\ell u}{c^2}(n^2-1),\qquad
N(u)\simeq\frac{2Lu}{c\lambda_0}(n^2-1)=\frac{4\ell u}{c\lambda_0}(n^2-1).
$$

Thus one shifted fringe corresponds to one cycle of [phase difference](phase-difference.md). If the stationary pattern has spatial [interference fringe spacing](interference-fringe-spacing.md) $d$, a simple readout model is $I(x)=I_0[1+\mathcal V\cos(2\pi x/d+2\pi N)]$, where $\mathcal V$ is the [interference visibility](interferometric-visibility.md). The maxima shift by $-dN$ with this choice of screen coordinate. A sign assigned to “rightward” motion depends on the image orientation; the magnitude in fringe units does not.

Reversing both flows gives $N(-u)=-N(u)$. The displacement between equal and opposite settings therefore has magnitude

$$
\left|N(u)-N(-u)\right|=2|N(u)|\simeq\frac{8\ell |u|}{c\lambda_0}(n^2-1).
$$

The factor $2$ from comparing opposite flows is additional to the factor $2$ already included in $L=2\ell$. Repeating a round trip in just one flowing tube would instead put a beam with the flow once and against it once; that geometry does not produce the two same-sign contributions drawn here.

## ↑ Ancestors (7)

1. [Fizeau experiment](fizeau-experiment.md)
2. [Velocity-addition formula](velocity-addition-formula.md)
3. [Lorentz transformation](lorentz-transformation.md)
4. [Special relativity](special-relativity-split.md)
5. [Branches of physics](branches-of-physics.md)
6. [Physics](physics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Fizeau experiment](fizeau-experiment.md)
