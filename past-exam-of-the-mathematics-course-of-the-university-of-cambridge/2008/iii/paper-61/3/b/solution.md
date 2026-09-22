<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

In [adaptive experimental quantum control](../../../../../../adaptive-experimental-quantum-control.md), parametrize a reproducible pulse by a finite real vector $c$, for example $f_c(t)=\sum_{j=1}^pc_jB_j(t)$ in a calibrated waveform basis. Prepare the same initial state for each trial, apply that pulse without feedback during the run, and estimate the objective $J(c)$ from repeated measurements. No accurate dynamical model is required if the laboratory can evaluate the objective.

One concrete algorithm is experimental finite-difference [gradient ascent](../../../../../../gradient-ascent.md). For every parameter, run trials at $c\pm\delta e_j$ and estimate

$$
g_j\simeq\frac{\overline J(c+\delta e_j)-\overline J(c-\delta e_j)}{2\delta}.
$$

Update $c$ to an admissible projection of $c+\eta g$, test the new pulse, and reduce the step size if performance deteriorates. Averaging many shots controls statistical noise; choose $\delta$ large enough for the difference to exceed the measurement uncertainty but small enough to approximate a [derivative](../../../../../../derivative.md). Repeat until no statistically significant improvement remains. Multiple starting pulses help explore distinct basins, but this does not guarantee a global optimum. Resource penalties and hardware restrictions belong in the objective or the admissible parameter set.

The feedback is across experimental runs: a measured objective chooses the next pulse. Each individual trial is [open-loop control](../../../../../../open-loop-control.md). This distinction matters because the algorithm does not require an instantaneous nondestructive state measurement on the system being controlled.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 61](../../../paper-61-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
