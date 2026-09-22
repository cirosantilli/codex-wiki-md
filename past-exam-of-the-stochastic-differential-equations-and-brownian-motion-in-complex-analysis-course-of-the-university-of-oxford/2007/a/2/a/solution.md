<h1 id="a/2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Apply [Itô's lemma](../../../../../ito-s-lemma.md) to $F(t,x)=e^{i\xi x+\xi^2t/2}$. Since $F_t=\xi^2F/2$, $F_x=i\xi F$ and $F_{xx}=-\xi^2F$, the drift terms cancel:

$$
dM_t=i\xi M_t\,dB_t,\qquad M_0=1.
$$

This is initially a [local martingale](../../../../../local-martingale.md). On every finite interval $[0,T]$,

$$
\mathbb E\int_0^T|i\xi M_s|^2ds
=\xi^2\int_0^Te^{\xi^2s}ds<\infty,
$$

so the [stochastic integral](../../../../../stochastic-integral.md) is a true [square-integrable martingale](../../../../../square-integrable-martingale.md). [Conditional expectation](../../../../../conditional-expectation.md) gives $\mathbb E(M_t\mid\mathcal F_s)=M_s$; divide by the nonzero $\mathcal F_s$-measurable factor $e^{i\xi B_s+\xi^2t/2}$ to obtain

$$
\boxed{\mathbb E(e^{i\xi(B_t-B_s)}\mid\mathcal F_s)=e^{-\xi^2(t-s)/2}.}
$$

## ↑ Ancestors (13)

1. [A](../a.md)
2. [2](../../2.md)
3. [A](../../../a.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../split.md)
6. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
