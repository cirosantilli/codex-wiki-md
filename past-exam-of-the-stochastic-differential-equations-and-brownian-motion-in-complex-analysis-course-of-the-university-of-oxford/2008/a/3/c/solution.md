<h1 id="a/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Condition on the Brownian path up to $t\leq T$. The independent normal increment $B_T-B_t$ has $\mathbb E\cos(B_T-B_t)=e^{-(T-t)/2}$ and zero expected sine. Hence

$$
M_t:=\mathbb E(\sin B_T\mid\mathcal F_t)
=e^{-(T-t)/2}\sin B_t.
$$

Apply [Itô's formula](../../../../../ito-s-lemma.md) to this expression. Its time derivative and second spatial derivative cancel, leaving

$$
dM_t=e^{-(T-t)/2}\cos B_t\,dB_t,\qquad M_0=0.
$$

Therefore the required representation is

$$
\boxed{\sin B_T=\int_0^T e^{-(T-s)/2}\cos B_s\,dB_s.}
$$

The bounded integrand is square integrable, and uniqueness follows from the [Itô isometry](../../../../../ito-isometry.md). The drift-containing decomposition in part (b) alone would not be the required representation as a constant plus one [stochastic integral](../../../../../stochastic-integral.md).

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [A](../../../a.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
