<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A simple example is

$$
\boxed{M_t=B_t^2-t}
$$

for a standard [Brownian motion](../../../../../../brownian-motion-split.md) $B$. The [Itô formula](../../../../../../ito-s-lemma.md) gives $M_t=2\int_0^tB_s\,dB_s$, a continuous square-integrable [martingale](../../../../../../martingale-split.md) on every finite horizon. For $h>0$, write $\Delta=B_{s+h}-B_s$, independent of the past and normal with variance $h$. Then

$$
M_{s+h}-M_s=2B_s\Delta+\Delta^2-h,
\qquad
\mathbb E[(M_{s+h}-M_s)^2\mid\mathcal F_s]=4B_s^2h+2h^2.
$$

Since $B_s^2=M_s+s$, this conditional second moment is already a nonconstant function of the [martingale](../../../../../../martingale-split.md)'s own past for $s>0$. The [tower property of conditional expectation](../../../../../../law-of-total-expectation.md) gives the same expression on conditioning on that own past. Were the increments independent, that conditional second moment would be constant. Thus the increments are not independent.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 38](../../../paper-38-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
