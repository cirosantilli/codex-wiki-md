<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Order $\Omega=\{0,1\}^E$ coordinatewise. The statement $\mu_1\ge_{\mathrm{st}}\mu_2$ means

$$
\int f\,d\mu_1\ge\int f\,d\mu_2
$$

for every real-valued [order-preserving function](../../../../../../order-preserving-function.md) $f$; equivalently, $\mu_1(A)\ge\mu_2(A)$ for every increasing event $A$. This is [stochastic domination of probability measures](../../../../../../stochastic-domination-of-probability-measures.md). For strictly positive laws, the [Holley condition](../../../../../../holley-condition.md) is the sufficient condition

$$
\boxed{\mu_1(\omega\vee\eta)\mu_2(\omega\wedge\eta)\ge\mu_1(\omega)\mu_2(\eta)\quad\text{for all }\omega,\eta.}
$$

Here join and meet are coordinatewise maximum and minimum. The [Holley inequality](../../../../../../holley-inequality.md) states that this condition implies the stated [stochastic domination](../../../../../../stochastic-domination-of-probability-measures.md).

For a single positive law, the [FKG lattice condition](../../../../../../fkg-lattice-condition.md) is

$$
\boxed{\mu(\omega\vee\eta)\mu(\omega\wedge\eta)\ge\mu(\omega)\mu(\eta).}
$$

We prove that it gives [positive association of random variables](../../../../../../positive-association-of-random-variables.md), namely $\operatorname{Cov}_\mu(f,g)\ge0$ for all increasing $f,g$. Fix such a $g$, and for $t\ge0$ form the strictly positive tilted law

$$
\mu_t(\omega)=\frac{e^{tg(\omega)}\mu(\omega)}{Z_t},\qquad Z_t=\sum_\omega e^{tg(\omega)}\mu(\omega).
$$

The lattice condition and $g(\omega\vee\eta)\ge g(\omega)$ imply

$$
\mu_t(\omega\vee\eta)\mu(\omega\wedge\eta)
\ge\frac{e^{tg(\omega)}}{Z_t}\mu(\omega)\mu(\eta)
=\mu_t(\omega)\mu(\eta).
$$

Thus the [Holley condition](../../../../../../holley-condition.md) applies to $\mu_t,\mu$, and $\mathbb E_{\mu_t}f\ge\mathbb E_\mu f$. Equality holds at $t=0$, so the right derivative there is nonnegative. Differentiating the finite sums gives

$$
\left.\frac{d}{dt}\mathbb E_{\mu_t}f\right|_{t=0}
=\mathbb E_\mu(fg)-\mathbb E_\mu f\,\mathbb E_\mu g.
$$

Hence

$$
\boxed{\operatorname{Cov}_\mu(f,g)\ge0,}
$$

which proves the requested [positive association of random variables](../../../../../../positive-association-of-random-variables.md). Neither $f$ nor $g$ needs to be nonnegative; the finite space makes all differentiations justified. This is the [exponential-tilt proof of positive association](../../../../../../exponential-tilt-proof-of-positive-association.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 37](../../../paper-37-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
