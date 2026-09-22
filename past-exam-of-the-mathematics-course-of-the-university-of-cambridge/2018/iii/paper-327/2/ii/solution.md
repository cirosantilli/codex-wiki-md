<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $T_q\varphi(x)=\sum_{k=0}^q\varphi^{(k)}(0)x^k/k!$ denote the [Taylor polynomial](../../../../../../taylor-polynomial.md) at zero. On $0<|x|<1$, the integrand defining the [Hadamard finite-part reciprocal-power distribution](../../../../../../hadamard-finite-part-reciprocal-power-distribution.md) is

$$
x^{-m}\bigl(\varphi(x)-T_{m-2}\varphi(x)\bigr)
=\frac{\varphi^{(m-1)}(0)}{(m-1)!}\frac1x
+x^{-m}\bigl(\varphi(x)-T_{m-1}\varphi(x)\bigr).
$$

The first term is odd, so it cancels under symmetric truncation. The [Taylor remainder](../../../../../../taylor-remainder.md) in the second term has absolute value at most $|x|^m\|\varphi^{(m)}\|_\infty/m!$. The integral near zero therefore has a finite limit. For $|x|\geq1$, the original terms are integrable: $x^{-m}\varphi$ has [compact support](../../../../../../compact-support.md), and each subtracted power has exponent $k-m\leq-2$.

This proves existence and linearity. It also gives the global estimate

$$
\begin{aligned}
|\langle\Lambda_m,\varphi\rangle|\leq{}&\frac2{m!}\|\varphi^{(m)}\|_\infty
+\frac2{m-1}\|\varphi\|_\infty\\
&+\sum_{k=0}^{m-2}\frac2{k!(m-k-1)}|\varphi^{(k)}(0)|.
\end{aligned}
$$

Thus

$$
\boxed{\Lambda_m\in\mathcal D'(\mathbb R),\qquad
\operatorname{ord}\Lambda_m\leq m.}
$$

In particular the [order of a distribution](../../../../../../order-of-a-distribution.md) is bounded by one integer on all [compact sets](../../../../../../compact-space.md), not merely separately on each of them.

For the recurrence, write the truncated [Hadamard finite-part integral](../../../../../../hadamard-finite-part-integral.md) as

$$
A_m(\varepsilon,\varphi)=\int_{|x|>\varepsilon}x^{-m}\varphi(x)\,dx
-C_m(\varepsilon,\varphi),
$$

where parity evaluates all subtraction integrals explicitly:

$$
C_m(\varepsilon,\varphi)=
2\sum_{\substack{0\leq k\leq m-2\\m-k\text{ even}}}
\frac{\varphi^{(k)}(0)}{k!(m-k-1)}\varepsilon^{k-m+1}.
$$

Set $C_1=0$ and $\Lambda_1=\operatorname{pv}(1/x)$. On the two truncated intervals, [integration by parts](../../../../../../integration-by-parts.md) gives

$$
\int_{|x|>\varepsilon}x^{-m}\varphi'(x)\,dx
=m\int_{|x|>\varepsilon}x^{-m-1}\varphi(x)\,dx
+\varepsilon^{-m}\bigl[(-1)^m\varphi(-\varepsilon)-\varphi(\varepsilon)\bigr].
$$

There are no boundary contributions at infinity. The coefficients of the subtraction terms satisfy

$$
mC_{m+1}(\varepsilon,\varphi)-C_m(\varepsilon,\varphi')
=2\sum_{\substack{0\leq k\leq m-1\\m-k\text{ odd}}}
\frac{\varphi^{(k)}(0)}{k!}\varepsilon^{k-m}.
$$

This is exactly the negative of the boundary term's [Taylor polynomial](../../../../../../taylor-polynomial.md) through degree $m$; the degree-$m$ term itself vanishes by parity. Hence

$$
\begin{aligned}
&A_m(\varepsilon,\varphi')-mA_{m+1}(\varepsilon,\varphi)\\
&\quad=\varepsilon^{-m}\left[
(-1)^m\bigl(\varphi(-\varepsilon)-T_m\varphi(-\varepsilon)\bigr)
-\bigl(\varphi(\varepsilon)-T_m\varphi(\varepsilon)\bigr)\right]
=O(\varepsilon).
\end{aligned}
$$

Taking the limit proves the full [distributional identity](../../../../../../distributional-identity.md)

$$
\boxed{\langle\Lambda_m,\varphi'\rangle=m\langle\Lambda_{m+1},\varphi\rangle,
\qquad \Lambda_m'=-m\Lambda_{m+1}.}
$$

The same calculation includes $m=1$. Starting with the [distributional derivative of the logarithmic modulus](../../../../../../distributional-derivative-of-the-logarithmic-modulus.md) from part (i), induction yields

$$
\boxed{\Lambda_m=\frac{(-1)^{m-1}}{(m-1)!}\left(\frac d{dx}\right)^m\log|x|,
\qquad c_m=\frac{(-1)^{m-1}}{(m-1)!}.}
$$

This identity holds on all of $\mathbb R$ as a [distributional identity](../../../../../../distributional-identity.md). It is stronger than matching the ordinary derivatives away from zero, which would leave possible differentiated [Dirac delta distributions](../../../../../../dirac-delta-function.md) at zero undetermined.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 327](../../../paper-327-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
