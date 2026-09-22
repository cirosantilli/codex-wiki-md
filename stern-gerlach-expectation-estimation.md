# Stern-Gerlach expectation estimation

↑ **Parent:** [Estimating a quantum expectation value](estimating-a-quantum-expectation-value.md)

A concrete idealized implementation uses a [Stern-Gerlach experiment](stern-gerlach-experiment.md) twice: a preparation filter along $\mathbf n=(\sin\theta,0,\cos\theta)$ passes only its plus [spin](spin.md) channel, and a $z$ analyzer resolves both output channels for many fresh atoms. This prepares the [spin one-half along an axis](spin-one-half-along-an-axis.md) state $|\psi_\theta\rangle$. The authored apparatus description uses slit collimation, a nonuniform [magnetic field](magnetic-field-split.md) with a pointed pole, and counters at the separated outputs.[The Feynman Lectures on Physics, Volume III, Chapter 5: Spin One, §5–1, figure 5–1 and the paragraph proposing output counters; §5–4, slit diffraction and internal-state limitations](the-feynman-lectures-on-physics-volume-iii-by-richard-feynman-and-others/chapter-5-spin-one.md) The two-channel [spin one-half](spin-one-half.md) preparation and analyzer are described separately; the source's recombining “improved” apparatus is explicitly idealized, so the setup here is a proposed estimation model, not a report of observed counts.[The Feynman Lectures on Physics, Volume III, Chapter 6: Spin One-Half, §6–2, figures 6–1 and 6–2: two beams, one-channel preparation, and a second analyzer; idealized apparatus qualification in §5–1 of the preceding chapter](the-feynman-lectures-on-physics-volume-iii-by-richard-feynman-and-others/chapter-6-spin-one-half.md)

Count every accepted analyzer event in its calibrated $+z$ or $-z$ channel and compute $\widehat\mu_N$ from the count difference. The [magnetic field](magnetic-field-split.md) gradient separates trajectories through their [magnetic moments](magnetic-dipole-moment.md); calibrated channel labels convert positions into [spin](spin.md) [eigenvalues](eigenvalue.md). The readout is a population imbalance, not an intermediate trajectory carrying [spin](spin.md) $\hbar\cos\theta/2$. Beam position also depends on flight time and field geometry, so averaging raw positions alone does not establish a calibrated [spin expectation value](spin-expectation-value.md).

As controls, feed known $|+z\rangle$ and $|-z\rangle$ preparations to check the channel assignment and leakage, hold the analyzer axis fixed, and repeat short blocks to check preparation drift. Measure background counts and relative channel efficiencies. With efficiencies $\eta_+$ and $\eta_-$ and negligible background, the detected plus fraction is

$$
p_+^{\rm det}=\frac{\eta_+p_+}{\eta_+p_++\eta_-(1-p_+)}.
$$

Unequal efficiencies bias the naive [sample mean](sample-mean.md), even for arbitrarily many counts. For example, $p_+=3/4$, $\eta_+=1$, and $\eta_-=1/2$ give detected fraction $6/7$ and naive mean $5\hbar/14$, rather than $\hbar/4$. Background, overlapping beams, detector saturation, angle misalignment, unwanted internal states, and preparation correlations require a better [measurement in quantum mechanics](quantum-measurement-split.md) model. Increasing $N$ only reduces the independent sampling contribution; it cannot remove these systematic errors. The selected preparation beam is the population being estimated, so losses in preparing it must be distinguished from losses in reading its two outcomes.

## ↑ Ancestors (9)

1. [Estimating a quantum expectation value](estimating-a-quantum-expectation-value.md)
2. [Expectation value](expectation-value.md)
3. [Observable](observable.md)
4. [Quantum state](quantum-state.md)
5. [Quantum system](quantum-system-split.md)
6. [Quantum mechanics](quantum-mechanics-split.md)
7. [Branches of physics](branches-of-physics.md)
8. [Physics](physics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Stern-Gerlach discrete and classical profiles](stern-gerlach-discrete-and-classical-profiles.md)
- [Stern-Gerlach experiment](stern-gerlach-experiment.md)
