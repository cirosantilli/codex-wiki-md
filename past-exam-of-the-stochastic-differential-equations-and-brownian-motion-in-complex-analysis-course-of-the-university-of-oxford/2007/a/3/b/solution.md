<h1 id="a/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Integrating the preceding differential gives $M(h_j)_T=1+\int_0^Th_j(s)M(h_j)_s\,dB_s$. Consequently $\mathbb E F=\sum_jc_j$, and the representation is

$$
\boxed{f_s=\sum_{j=1}^Nc_jh_j(s)M(h_j)_s,\qquad
F=\sum_jc_j+\int_0^Tf_s\,dB_s.}
$$

The process is continuous and [adapted](../../../../../adapted-process.md), hence [progressively measurable](../../../../../progressive-measurability.md), and the finite-sum inequality together with the previous second-moment estimate gives $\mathbb E\int_0^T|f_s|^2ds<\infty$.

If $g$ is another square-integrable predictable [integrand](../../../../../integrand.md) with the same representation, [Itô isometry](../../../../../ito-isometry.md) gives

$$
0=\mathbb E\left|\int_0^T(f_s-g_s)dB_s\right|^2
=\mathbb E\int_0^T|f_s-g_s|^2ds.
$$

Thus **uniqueness is up to $ds\otimes d\mathbb P$ [null sets](../../../../../null-set.md) in the square-integrable [integrand](../../../../../integrand.md) class**. Pointwise uniqueness is impossible: changing a value at one deterministic time changes no [Itô integral](../../../../../ito-integral.md). Square integrability is the natural class for this $L^2$ representation and is needed for this uniqueness argument; the mere word [adapted](../../../../../adapted-process.md) does not by itself specify an integrable [stochastic integral](../../../../../stochastic-integral.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
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
