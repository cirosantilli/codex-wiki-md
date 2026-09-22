<h1 id="3/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

One form of the [Feynman-Kac formula](../../../../../../feynman-kac-formula.md) is the following. For bounded sufficiently regular $f,V$ and

$$
u(t,x)=\mathbb E_x\left[
 e^{-\int_0^tV(B_s)ds}f(B_t)
\right],
$$

one has

$$
\partial_tu=\frac12\Delta u-Vu,
\qquad u(0,x)=f(x).
$$

Conversely, a bounded classical solution has this representation. To prove it, fix $t$ and apply [Itô formula](../../../../../../ito-s-lemma.md) to

$$
e^{-\int_0^sV(B_r)dr}u(t-s,B_s),\qquad0\leq s\leq t.
$$

The PDE cancels its drift. The remaining stochastic integral is a martingale, so taking expectations at $s=0,t$ gives the representation; the converse follows by the same calculation and uniqueness for the parabolic boundary-value problem.

## ↑ Ancestors (11)

1. [3](../3.md)
2. [3](../../3.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
