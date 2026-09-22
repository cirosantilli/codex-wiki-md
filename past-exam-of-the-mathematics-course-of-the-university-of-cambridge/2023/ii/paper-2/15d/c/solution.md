<h1 id="15d/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The two registers start in $|0\rangle|0\rangle$. A [quantum Fourier transform](../../../../../../quantum-fourier-transform.md) on the first and evaluation of $f$ give

$$
|0\rangle|0\rangle
\longmapsto
\frac14\sum_{x=0}^{15}|x\rangle|0\rangle
\longmapsto
\frac14\sum_{x=0}^{15}|x\rangle|f(x)\rangle.
$$

The first [measurement](../../../../../../quantum-measurement-in-the-computational-basis.md), on the function register, returns $1$. The compatible inputs are $1,5,9,13$, so the normalized state becomes

$$
\frac12\bigl(|1\rangle+|5\rangle+|9\rangle+|13\rangle\bigr)|1\rangle.
$$

Apply $\operatorname{QFT}_{16}$ to the first register and put $\omega=e^{2\pi i/16}$. Its state is

$$
\frac18\sum_{y=0}^{15}
\omega^y\left(1+\omega^{4y}+\omega^{8y}+\omega^{12y}\right)|y\rangle.
$$

The geometric sum vanishes unless $4\mid y$. Thus this is

$$
\frac12\left(
|0\rangle+i|4\rangle-|8\rangle-i|12\rangle
\right),
$$

up to the unchanged second register. The outcomes $0,4,8,12$ each have probability $1/4$, in accordance with the [quantum Fourier transform of a periodic coset state](../../../../../../quantum-fourier-transform-of-a-periodic-coset-state.md).

For the stated second outcome,

$$
\frac{12}{16}=\frac34.
$$

The [continued-fraction algorithm](../../../../../../continued-fraction-algorithm.md) therefore returns denominator $4$. Since the numerator $3$ is coprime to the true period, [exact period recovery from a Fourier sample](../../../../../../exact-period-recovery-from-a-fourier-sample.md) succeeds, and direct evaluation confirms that the least period is

$$
\boxed{r=4}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [15D](../../15d.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
