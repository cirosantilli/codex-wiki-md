<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For short times, survival under [unitary time evolution](../../../../unitary-time-evolution.md) is $1-(\Delta H)^2t^2/\hbar^2+O(t^3)$. Dividing a fixed time into $N$ intervals and projecting back after each gives survival approaching one as $N\to\infty$. This suppression of departure by repeated [projective measurements](../../../../projective-measurement.md) is the [quantum Zeno effect](../../../../quantum-zeno-effect.md).

For [measurement-guided Zeno transfer](../../../../measurement-guided-zeno-transfer.md), rotate the measured basis gradually to transport a known state. Let

$$
|b_j\rangle=\cos\theta_j|0\rangle+\sin\theta_j|1\rangle,\quad
|b_j^\perp\rangle=-\sin\theta_j|0\rangle+\cos\theta_j|1\rangle,\quad
\theta_j=\frac{j\pi}{2N}.
$$

Measure in these orthonormal bases successively for $j=1,\ldots,N$. Starting in $|0\rangle=|b_0\rangle$, the probability to follow the $b_j$ outcome at every step is

$$
\boxed{P_{\rm follow}=\cos^{2N}\left(\frac{\pi}{2N}\right)\longrightarrow1.}
$$

Its final state is $|b_N\rangle=|1\rangle$. If every outcome is retained without postselection, the final probability for $|1\rangle$ is $[1+\cos^N(\pi/N)]/2$, also approaching one; histories with two switches can return to that branch. These two finite-$N$ probabilities should not be confused.

For a general unknown input, the same slowly turning measurements first resolve its amplitudes into the two branches, then drag each branch separately. In the large-$N$ limit, after discarding the records,

$$
\boxed{\rho_{\rm out}\longrightarrow|\alpha|^2|1\rangle\langle1|+|\beta|^2|0\rangle\langle0|.}
$$

The first basis approaches the computational one as $N$ grows. Inserting an initial computational measurement makes this branch decomposition exact at the outset, without changing the limiting result. Relative phase is lost, so this procedure transports a known basis state with high probability rather than implementing a coherent [Pauli X gate](../../../../pauli-x-gate.md) on an arbitrary [qubit](../../../../qubit.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the laser science and quantum information processing course of the University of Oxford](../../../split.md)
5. [Laser science and quantum information processing course of the University of Oxford](../../../../laser-science-and-quantum-information-processing-course-of-the-university-of-oxford.md)
6. [Year 4 of the physics course of the University of Oxford](../../../../year-4-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
