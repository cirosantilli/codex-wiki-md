<h1 id="15c/d/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

This circuit is the [swap test](../../../../../../../swap-test.md). If the two pure states are identical up to a physically irrelevant [global phase](../../../../../../../global-phase.md), then $|\langle\psi|\phi\rangle|=1$ and outcome one never occurs. If they are distinct, then $|\langle\psi|\phi\rangle|<1$ and each run produces outcome one with positive probability $p_1$.

Run the circuit independently on fresh copies. Observing even one outcome one proves that the states differ. If no one occurs in $N$ runs, that event has probability

$$
p_0^N
=\left[\frac{1+|\langle\psi|\phi\rangle|^2}{2}\right]^N
$$

when the states differ, which tends to zero as $N\to\infty$. Repetition therefore distinguishes equality from inequality with arbitrarily high probability.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [D](../../d.md)
3. [15C](../../../15c.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
