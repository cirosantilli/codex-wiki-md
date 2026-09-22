# Chirped Gaussian wave packet

↑ **Parent:** [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md)

A [chirped Gaussian wave packet](chirped-gaussian-wave-packet.md) adds a quadratic [quantum phase](quantum-phase.md) to the zero-mean [Gaussian wave packet](gaussian-wave-packet.md) already evaluated above. Here $\sigma>0$ and $\kappa$ is a real dimensionless parameter. Its [probability density function](probability-density-function.md) $|\psi_{\sigma,\kappa}(x)|^2$ is unchanged for every $\kappa$, so $\langle x\rangle=0$ and $(\Delta x)^2=\sigma^2$. Nevertheless, applying the [momentum operator](momentum-operator.md) gives

$$
p\psi_{\sigma,\kappa}=\frac{\hbar(\kappa+i)x}{2\sigma^2}\psi_{\sigma,\kappa},
\qquad \langle p\rangle=0,
\qquad (\Delta p)^2=\|p\psi_{\sigma,\kappa}\|^2=\frac{\hbar^2(1+\kappa^2)}{4\sigma^2}.
$$

The sign of the [quantum covariance](quantum-covariance.md) follows directly, without assigning a classical trajectory to the [wavefunction](wave-function-split.md):

$$
\langle xp\rangle=\frac{\hbar}{2}(\kappa+i),
\qquad C_{xp}=\operatorname{Re}\langle xp\rangle=\frac{\hbar\kappa}{2},
\qquad r=\frac{C_{xp}}{\Delta x\,\Delta p}=\frac{\kappa}{\sqrt{1+\kappa^2}}.
$$

Here $r$ is a normalized symmetrized [quantum covariance](quantum-covariance.md), analogous to a [correlation coefficient](pearson-correlation-coefficient.md). Positive $\kappa$ gives positive $C_{xp}$, and reversing $\kappa$ reverses $C_{xp}$ while leaving both [variances](variance-split.md) unchanged. In the negative-exponent [Fourier transform](fourier-transform-split.md) convention used above, the [momentum](momentum-split.md) density is

$$
|\widetilde\psi_{\sigma,\kappa}(p)|^2
=\sqrt{\frac{2\sigma^2}{\pi\hbar^2(1+\kappa^2)}}
\exp\!\left(-\frac{2\sigma^2p^2}{\hbar^2(1+\kappa^2)}\right).
$$

Consequently the [quantum uncertainty](quantum-uncertainty.md) product and the [covariance matrix](covariance-matrix.md) [determinant](determinant.md) tell different stories:

$$
\Delta x\,\Delta p=\frac{\hbar}{2}\sqrt{1+\kappa^2},
\qquad
\det\Sigma=\frac{\hbar^2(1+\kappa^2)}4-\frac{\hbar^2\kappa^2}4=\frac{\hbar^2}4.
$$

Every member of this [pure state](pure-state.md) family saturates the [Robertson-Schrödinger uncertainty relation](robertson-schrodinger-uncertainty-relation.md). Only $\kappa=0$ saturates the [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md) for this fixed pair of [position](position.md) and [momentum](momentum-split.md) axes. Thus being a [Gaussian wave packet](gaussian-wave-packet.md) alone does not imply a minimum $\Delta x\,\Delta p$.

For a concrete comparison, choose a reference [length](length.md) $L$, put $X=x/L$, $P=pL/\hbar$, and set $\sigma=L$. The choices $\kappa=0,+2,-2$ all have $(\Delta X)^2=1$, but give $(\Delta P)^2=1/4,5/4,5/4$ and $C_{XP}=0,+1,-1$, respectively. The two nonzero cases have $r=\pm2/\sqrt5$ and product $\sqrt5/2$; all three [covariance matrices](covariance-matrix.md) have [determinant](determinant.md) $1/4$.

<a id="image-quadratic-phase-preserves-the-position-density-but-broadens-the-momentum-density-opposite-chirps-tilt-covariance-ellipses-in-opposite-directions-while-preserving-their-area"></a>
![](chirped-gaussian-covariance-ellipse.png)

**[Figure 7](#image-quadratic-phase-preserves-the-position-density-but-broadens-the-momentum-density-opposite-chirps-tilt-covariance-ellipses-in-opposite-directions-while-preserving-their-area). Quadratic phase preserves the position density but broadens the momentum density: opposite chirps tilt covariance ellipses in opposite directions while preserving their area**.

The [phase space](phase-space.md) curves in the figure satisfy $z^T\Sigma^{-1}z=1$ in the dimensionless coordinates, where $z=(X,P)^T$. They display second moments, not observed simultaneous [position](position.md) and [momentum](momentum-split.md) pairs. Their common area is $\pi\sqrt{\det\Sigma}=\pi/2$, although their coordinate projections differ.

This distinction is useful for predicting focusing. Under [free particle](free-particle.md) evolution with [mass](mass.md) $m$, $x(t)=x(0)+tp(0)/m$, so

$$
(\Delta x(t))^2=\sigma^2+\frac{2t}{m}C_{xp}+\frac{t^2}{m^2}(\Delta p)^2.
$$

A negative chirp initially narrows the [position](position.md) distribution; positive chirp initially broadens it. For $\kappa<0$, the minimum occurs at $t_*=-2m\sigma^2\kappa/[\hbar(1+\kappa^2)]>0$ and has [variance](variance-split.md) $\sigma^2/(1+\kappa^2)$. At that time the [quantum covariance](quantum-covariance.md) vanishes, and the unchanged [momentum](momentum-split.md) spread gives $\Delta x(t_*)\,\Delta p=\hbar/2$. The extra initial product was a usable position-momentum correlation, not extra [measurement backaction](measurement-backaction.md).

## ↑ Ancestors (6)

1. [Heisenberg uncertainty relation](heisenberg-uncertainty-relation.md)
2. [Robertson uncertainty principle](robertson-uncertainty-principle.md)
3. [Quantum theory](quantum-theory-split.md)
4. [Branches of physics](branches-of-physics.md)
5. [Physics](physics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Chirped Gaussian wave packet](chirped-gaussian-wave-packet.md)
- [Solution](past-exam-of-the-physics-a-course-of-the-university-of-cambridge/2019/paper-1/section-c/c10/solution.md)
