# Spin expectation value

↑ **Parent:** [Expectation value](expectation-value.md)

For [spin one-half](spin-one-half.md), choose the normalized [spin](spin.md) [eigenstates](eigenstate.md) $|+z\rangle,|-z\rangle$ with $S_z|\pm z\rangle=\pm(\hbar/2)|\pm z\rangle$. The [spin one-half along an axis](spin-one-half-along-an-axis.md) [pure state](pure-state.md) in the $xz$ plane is

$$
|\psi_\theta\rangle=\cos(\theta/2)|+z\rangle+\sin(\theta/2)|-z\rangle,\qquad 0\leq\theta\leq\pi.
$$

Its [norm](norm.md) is one because the two [eigenstates](eigenstate.md) are [orthogonal](orthogonal-vectors.md) and $\cos^2(\theta/2)+\sin^2(\theta/2)=1$. Applying the [Born rule](born-rule.md) to a $z$ [projective measurement](projective-measurement.md) gives

$$
p_+=\cos^2(\theta/2)=\frac{1+\cos\theta}{2},\qquad
p_-=\sin^2(\theta/2)=\frac{1-\cos\theta}{2}.
$$

Consequently the [expectation value](expectation-value.md), second moment, and [variance](variance-split.md) are

$$
\langle S_z\rangle=\frac{\hbar}{2}(p_+-p_-)=\frac{\hbar}{2}\cos\theta,\qquad
\langle S_z^2\rangle=\frac{\hbar^2}{4},\qquad
(\Delta S_z)^2=\frac{\hbar^2}{4}\sin^2\theta.
$$

At $\theta=\pi/3$, the outcome [probabilities](probability.md) are $3/4$ and $1/4$, the mean is $\hbar/4$, and the [variance](variance-split.md) is $3\hbar^2/16$. Every individual outcome remains $\pm\hbar/2$. At $\theta=\pi/2$, the mean is zero and the [variance](variance-split.md) is maximal, $\hbar^2/4$. At either pole, one outcome has [probability](probability.md) one and the [variance](variance-split.md) vanishes.

<a id="image-spin-expectation-value-between-the-two-possible-s-z-outcomes"></a>
![](spin-expectation-outcome-probabilities.png)

**[Figure 5](#image-spin-expectation-value-between-the-two-possible-s-z-outcomes). Spin expectation value between the two possible $S_z$ outcomes**. [Source](spin-expectation-outcome-probabilities.py). Original calculated [Born rule](born-rule.md) distributions at three preparation angles. Bar heights are outcome [probabilities](probability.md); the dashed orange line marks the [expectation value](expectation-value.md), whose horizontal position is usually not an allowed outcome. Spin values are expressed in units of the reduced [Planck constant](planck-constant.md). No bars represent experimental observations.

The diagonal [mixed state](mixed-state.md) $\rho_{\rm diag}=p_+|+z\rangle\langle+z|+p_-|-z\rangle\langle-z|$ has the same $S_z$ [probabilities](probability.md), [expectation value](expectation-value.md), and [variance](variance-split.md) as $|\psi_\theta\rangle$. It is nevertheless a different [quantum state](quantum-state.md) for $0<\theta<\pi$: the displayed [pure state](pure-state.md) has $\langle S_x\rangle=\hbar\sin\theta/2$, while $\rho_{\rm diag}$ has $\langle S_x\rangle=0$. A single component's mean does not reveal all relative [quantum phases](quantum-phase.md) or establish [purity of a density operator](purity-of-a-density-operator.md).

## ↑ Ancestors (8)

1. [Expectation value](expectation-value.md)
2. [Observable](observable.md)
3. [Quantum state](quantum-state.md)
4. [Quantum system](quantum-system-split.md)
5. [Quantum mechanics](quantum-mechanics-split.md)
6. [Branches of physics](branches-of-physics.md)
7. [Physics](physics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Estimating a quantum expectation value](estimating-a-quantum-expectation-value.md)
- [Rashba spin texture](rashba-spin-texture.md)
- [Spin expectation value](spin-expectation-value.md)
- [Spin texture](spin-texture.md)
- [Stern-Gerlach expectation estimation](stern-gerlach-expectation-estimation.md)
