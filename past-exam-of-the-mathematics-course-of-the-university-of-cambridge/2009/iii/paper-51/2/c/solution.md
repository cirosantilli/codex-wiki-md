<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $N\geq2$, induction using the [Grover rotation angle](../../../../../../grover-rotation-angle.md) gives

$$
G^k|\psi_A\rangle=\sin((2k+1)\theta)|a\rangle+\cos((2k+1)\theta)|\omega\rangle.
$$

The [quantum measurement in the computational basis](../../../../../../quantum-measurement-in-the-computational-basis.md) therefore returns $a$ with [probability](../../../../../../probability.md) $\sin^2((2k+1)\theta)$. Since $0<\theta\leq\pi/4$, the first angle interval attaining the required success is

$$
\frac\pi2-\theta\ \leq\ (2k+1)\theta\ \leq\ \frac\pi2+\theta.
$$

The [first successful Grover iterate](../../../../../../first-successful-grover-iterate.md) is consequently

$$
\boxed{k_{\min}=\left\lceil\frac{\pi}{4\theta}-1\right\rceil
=\left\lceil\frac{\pi}{4\theta}\right\rceil-1.}
$$

Indeed, this is the first integer at or above the lower endpoint requirement $k\geq\pi/(4\theta)-1$. The inequality $\lceil t-1\rceil<t$ also implies $(2k_{\min}+1)\theta<\pi/2+\theta$, so this iterate cannot overshoot the first success interval. Every smaller nonnegative integer lies before that interval and fails the threshold. Finally, $\arcsin u>u$ for $0<u<1$, so

$$
\boxed{k_{\min}<\frac{\pi}{4\theta}<\frac{\pi\sqrt N}{4}.}
$$

For the singleton case $N=1$, measuring the initial state already returns $a$ with certainty, and $k_{\min}=0<\pi/4$. For $N=2$, the requested threshold is only $1/2$, so zero iterations already suffice. These boundary cases agree with the search guarantee.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 51](../../../paper-51-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
