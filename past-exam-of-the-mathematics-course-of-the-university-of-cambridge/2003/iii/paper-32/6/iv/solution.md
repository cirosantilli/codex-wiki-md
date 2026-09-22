<h1 id="6/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

The correct state in a general [Gaussian forward-rate field](../../../../../../gaussian-forward-rate-field.md) is the whole current curve. In time-to-maturity coordinates $g_t(x)=f(t,t+x)$, assume deterministic time-homogeneous volatility $\sigma(x)\in H$. Set $A(x)=\langle\sigma(x),\int_0^x\sigma(u)du\rangle$. The [Musiela forward-curve equation](../../../../../../musiela-forward-curve-equation.md) is

$$
\boxed{dg_t(x)=[\partial_xg_t(x)+A(x)]dt+\langle\sigma(x),dW_t\rangle.}
$$

Under the appropriate maturity differentiability, or in its mild interpretation on a suitable function space, its solution is

$$
g_t(x)=g_0(x+t)+\int_0^t A(x+t-s)ds+\int_0^t\langle\sigma(x+t-s),dW_s\rangle.
$$

For any future interval, the shifted current curve determines the deterministic part and future Brownian increments are independent of past information. This proves that the curve-valued process is time-homogeneous [Markov](../../../../../../markov-property.md). General observation-time-dependent deterministic volatility instead gives a time-inhomogeneous Markov curve. A low-dimensional state requires more: the maturity functions carrying the randomness must close under the shift evolution. Finitely many Brownian drivers by itself does not ensure that the short rate is Markov.

For a precise obstruction, take two independent stationary [Ornstein-Uhlenbeck processes](../../../../../../ornstein-uhlenbeck-process.md) $Z^1,Z^2$ with distinct positive decay parameters $a_1,a_2$, and let $r_t=m+Z_t^1+Z_t^2$. Its centered covariance is $C(h)=c_1e^{-a_1|h|}+c_2e^{-a_2|h|}$ with $c_1,c_2>0$. A stationary scalar Gaussian Markov process must satisfy the [covariance criterion for a stationary Gaussian Markov process](../../../../../../covariance-criterion-for-a-stationary-gaussian-markov-process.md):

$$
C(s+t)C(0)=C(s)C(t),\qquad s,t\geq0.
$$

Indeed Gaussian conditioning gives $\mathbb E[r_{s+t}-m\mid r_s]=C(t)(r_s-m)/C(0)$; if the present is a Markov state, conditioning the future also on the earlier $r_0$ cannot change that mean. Multiplication by $r_0-m$ and taking expectations yields the equation. For the two-factor covariance the difference of its two sides is

$$
c_1c_2(e^{-a_1s}-e^{-a_2s})(e^{-a_1t}-e^{-a_2t})\ne0\quad(s,t>0).
$$

So the short rate alone is not Markov, although the two-dimensional factor process is. Distinct exponentially decaying HJM volatility components realize such a multi-factor Gaussian curve model.

Stationarity is an additional condition, not a consequence of Gaussianity or time-homogeneity. A [stationary Gaussian forward curve](../../../../../../stationary-gaussian-forward-curve.md) for the time-homogeneous model can be constructed when

$$
K(x,y)=\int_0^\infty\langle\sigma(x+s),\sigma(y+s)\rangle ds
$$

is finite and the deterministic mean satisfies $m'(x)+A(x)=0$. Initialize $g_0$ with mean $m$ and covariance $K$, independently of future noise. The mild solution has the same mean, since $m(x+t)+\int_0^t A(x+s)ds=m(x)$. Its covariance is

$$
K(x+t,y+t)+\int_0^t\langle\sigma(x+s),\sigma(y+s)\rangle ds=K(x,y).
$$

Thus its one-time Gaussian curve distribution is invariant, and the time-homogeneous transition law makes all time-shifted finite-dimensional distributions invariant as well. The initial field can explicitly be built from an independent noise on negative times using the same square-integrable kernels.

For example, $\sigma_j(x)=\eta_je^{-a_jx}$ with $a_j>0$ gives

$$
K(x,y)=\sum_j\frac{\eta_j^2}{2a_j}e^{-a_j(x+y)},\qquad g_t(x)=m(x)+\sum_j e^{-a_jx}Z_t^j,
$$

where $dZ_t^j=-a_jZ_t^jdt+\eta_jdW_t^j$ and the factors start in their stationary normal laws. This is a finite-dimensional Markov realization when the sum is finite. In contrast, a nonzero constant maturity volatility makes $K(x,x)$ infinite, excluding a finite-variance stationary curve of this form. A deterministic initial curve is generally nonstationary even when a stationary distribution exists. These distinctions separate **Gaussianity, Markov state sufficiency, and stationarity**.

## ↑ Ancestors (11)

1. [Iv](../iv.md)
2. [6](../../6.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
