# Amplitude amplification

↑ **Parent:** [Quantum theory](quantum-theory-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Amplitude_amplification)

[Amplitude amplification](amplitude-amplification.md) increases the [probability](probability.md) of obtaining an answer accepted by a specified [Boolean function](boolean-function.md). It requires a coherent preparation $A$, its inverse, and a [marked-state phase oracle](marked-state-phase-oracle.md) that negates accepted components. Alternating that sign change with a [reflection operator](reflection-operator.md) about the prepared state directs [interference](interference-wave-propagation.md) toward the accepted subspace. Brassard, Høyer, Mosca, and Tapp developed the general framework, extending [Grover's algorithm](grover-s-algorithm.md) beyond a [uniform quantum superposition](uniform-quantum-superposition.md). [Brassard et al., Quantum Amplitude Amplification and Estimation, 2000, §2](https://arxiv.org/abs/quant-ph/0005055).

If a normalized [quantum state](quantum-state.md) has good amplitude $\sin\theta$, the product of the reflection in the bad axis and the reflection in the state line rotates its good-bad plane by $2\theta$. After $k$ iterations the good [probability](probability.md) is

$$
\sin^2((2k+1)\theta),
$$

so $O(1/\sin\theta)$ iterations raise a small good amplitude close to one. Success subsequently oscillates, making the stopping time part of the algorithm.

Compute the [exact Grover search on four entries](exact-grover-search-on-four-entries.md) directly. Order the [computational basis](computational-basis.md) as $00,01,10,11$ and mark $11$. The [Hadamard transform](hadamard-transform.md) prepares amplitudes $(1/2,1/2,1/2,1/2)$. The [marked-state phase oracle](marked-state-phase-oracle.md) changes these to $(1/2,1/2,1/2,-1/2)$, whose [arithmetic mean](arithmetic-mean.md) is $\overline a=1/4$. The [Grover diffusion operator](grover-diffusion-operator.md) performs [inversion about the mean](inversion-about-the-mean.md):

$$
a_x\longmapsto2\overline a-a_x,\qquad
\left(\tfrac12,\tfrac12,\tfrac12,-\tfrac12\right)\longmapsto(0,0,0,1).
$$

The three unmarked amplitudes become $1/2-1/2=0$, while the marked amplitude becomes $1/2-(-1/2)=1$. All three stages have squared [norm](norm.md) one. Here $\sin\theta=1/2$, so $\theta=\pi/6$ and one iteration gives $\sin^2(3\theta)=1$, agreeing with the explicit calculation.

<a id="image-one-grover-iteration-on-four-states-a-phase-flip-followed-by-reflection-about-the-mean-concentrates-all-amplitude-on-the-marked-state"></a>
![](four-state-amplitude-amplification.png)

**[Figure 2](#image-one-grover-iteration-on-four-states-a-phase-flip-followed-by-reflection-about-the-mean-concentrates-all-amplitude-on-the-marked-state). One Grover iteration on four states: a phase flip followed by reflection about the mean concentrates all amplitude on the marked state**.

Grover's original search paper was submitted on 29 May 1996; its algorithm combines selective sign changes with [inversion about the mean](inversion-about-the-mean.md). The example exposes the beauty of that construction: a change initially invisible to [computational-basis measurement](quantum-measurement-in-the-computational-basis.md) becomes complete cancellation of every wrong answer. [Grover, A fast quantum mechanical algorithm for database search, 1996, §§3–4](https://arxiv.org/abs/quant-ph/9605043).

The [marked-state phase oracle](marked-state-phase-oracle.md) is an assumed operation, whose implementation cost must be counted. [Computational-basis measurement](quantum-measurement-in-the-computational-basis.md) yields a candidate label, here $11$; using it to retrieve a record requires the relevant data access. Preparing a [quantum superposition](quantum-superposition.md) does not make all its entries available as classical outputs. The improvement concerns the number of oracle queries needed to obtain an accepted label.

**Table of contents**

- [Nearest-integer stopping for amplitude amplification](nearest-integer-stopping-for-amplitude-amplification.md)
- [Two-dimensional matrix for phase amplitude amplification](two-dimensional-matrix-for-phase-amplitude-amplification.md)
- [Exact amplitude amplification](exact-amplitude-amplification.md)
  - [Known-state success dilution for exact amplitude amplification](known-state-success-dilution-for-exact-amplitude-amplification.md)
  - [Phase-matched amplitude amplification](phase-matched-amplitude-amplification.md)
- [Geometric amplitude-amplification schedule](geometric-amplitude-amplification-schedule.md)

## ↑ Ancestors (4)

1. [Quantum theory](quantum-theory-split.md)
2. [Branches of physics](branches-of-physics.md)
3. [Physics](physics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (21)

- [Amplitude amplification](amplitude-amplification.md)
- [Known-state success dilution for exact amplitude amplification](known-state-success-dilution-for-exact-amplitude-amplification.md)
- [Marked density under a permutation](marked-density-under-a-permutation.md)
- [Nearest-integer stopping for amplitude amplification](nearest-integer-stopping-for-amplitude-amplification.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-53/4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-58/4/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-58/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-61/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-324/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-324/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-324/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-324/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/ii/paper-3/15e/g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-324/2/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-324/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-324/2/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-324/3/a/iv/solution.md)
- [Permutation-preimage quantum search](permutation-preimage-quantum-search.md)
- [Quantum theory](quantum-theory-split.md)
