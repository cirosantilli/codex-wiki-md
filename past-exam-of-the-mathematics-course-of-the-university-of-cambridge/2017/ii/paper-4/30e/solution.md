<h1 id="30e/solution">Solution</h1>

↑ **Parent:** [30E](../30e.md)

Put $q=\mu^2-1/4$ and $S=\log y$. The [differential equation](../../../../../differential-equation-split.md) becomes the [Riccati equation](../../../../../riccati-equation.md) $S''+(S')^2=1/4+q/x^2$. The inverse-power exponential hierarchy begins with

$$
(S_0')^2=\frac14,\qquad2S_0'S_1'+S_0''=0,
$$

so choose $S_0=\varepsilon x/2$, $S_1=0$ with $\varepsilon=\pm1$; additive constants specify the overall normalization. At order $x^{-2}$, $2S_0'S_2'=q/x^2$, and at subsequent orders

$$
2S_0'S_j'+S_{j-1}''+\sum_{r=2}^{j-2}S_r'S_{j-r}'=0,\qquad j\geq3.
$$

These equations are formally equivalent coefficient by coefficient; the order-zero transport term happens to be constant, so its chosen zero value is not interpreted as a literal denominator in a successive-ratio hypothesis. The ansatz $S_j=c_jx^{-(j-1)}$ is consistent for $j\geq2$, with

$$
\boxed{c_2=-\varepsilon q,\qquad
c_j=\varepsilon\left[(j-2)c_{j-1}+\frac1{j-1}\sum_{r=2}^{j-2}(r-1)(j-r-1)c_rc_{j-r}\right],\quad j\geq3.}
$$

Empty sums are zero. In particular $c_3=-q$, which agrees with direct expansion of the [Riccati equation](../../../../../riccati-equation.md).

Exponentiating the inverse-power series gives $y_\varepsilon\sim e^{\varepsilon x/2}\sum_{j\geq0}A_j^\varepsilon x^{-j}$ with $A_0=1$. Substitute this amplitude series into $u''+\varepsilon u'=qx^{-2}u$ to obtain

$$
\boxed{A_{j+1}^\varepsilon=\frac{\varepsilon[j(j+1)-q]}{j+1}A_j^\varepsilon,\qquad
A_1^\varepsilon=-\varepsilon q,\quad A_2^\varepsilon=\frac{q(q-2)}2.}
$$

Formal matching alone does not prove existence of actual solutions with these asymptotics. Here actual solutions are obtained from the [Modified Bessel differential equation](../../../../../modified-bessel-differential-equation.md) and the [large-argument asymptotic expansion of a modified Bessel function](../../../../../large-argument-asymptotic-expansion-of-a-modified-bessel-function.md): substituting $y=\sqrt x\,w(x/2)$ yields solutions $\sqrt\pi\sqrt x\,I_\mu(x/2)$ and $\sqrt{x/\pi}\,K_\mu(x/2)$, using the [Modified Bessel function of the first kind](../../../../../modified-bessel-function-of-the-first-kind.md) and [Modified Bessel function of the second kind](../../../../../modified-bessel-function-of-the-second-kind.md), whose positive-real-axis [asymptotic expansions](../../../../../asymptotic-expansion.md) have precisely these normalized growing and decaying series. They are [linearly independent](../../../../../linear-independence.md). The series need not converge; it is an [asymptotic expansion](../../../../../asymptotic-expansion.md) with a remainder after each fixed truncation. When $q=j(j+1)$ the amplitude recurrence terminates.

## ↑ Ancestors (10)

1. [30E](../30e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ii](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
