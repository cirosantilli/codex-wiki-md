<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the unscaled [Finite Fresnel integrals](../../../../../../finite-fresnel-integrals.md) of this paper. Termwise integration of the absolutely convergent [Taylor series](../../../../../../taylor-series.md) for sine and cosine gives the full small-argument expansions

$$
C(\lambda)=\sum_{n=0}^{\infty}\frac{(-1)^n\lambda^{4n+1}}{(2n)!(4n+1)},\qquad S(\lambda)=\sum_{n=0}^{\infty}\frac{(-1)^n\lambda^{4n+3}}{(2n+1)!(4n+3)}.
$$

In particular,

$$
\boxed{C(\lambda)=\lambda-\frac{\lambda^5}{10}+\frac{\lambda^9}{216}+O(\lambda^{13}),\qquad S(\lambda)=\frac{\lambda^3}{3}-\frac{\lambda^7}{42}+\frac{\lambda^{11}}{1320}+O(\lambda^{15}).}
$$

These [Taylor series](../../../../../../taylor-series.md) converge at every finite argument, although cancellation makes them unattractive for large arguments.

For the large-argument [asymptotic expansions](../../../../../../asymptotic-expansion.md), combine the two [Finite Fresnel integrals](../../../../../../finite-fresnel-integrals.md) into $C+iS$. The standard [Fresnel integral](../../../../../../fresnel-integral.md) gives

$$
\int_0^\infty e^{it^2}dt=e^{i\pi/4}\frac{\sqrt\pi}{2}=A(1+i),\qquad A=\sqrt{\frac\pi8}.
$$

For the tail $J(\lambda)=\int_\lambda^\infty e^{it^2}dt$, [integration by parts](../../../../../../integration-by-parts.md) using $(e^{it^2})'=2it e^{it^2}$ gives

$$
J(\lambda)\sim e^{i\lambda^2}\sum_{n\ge0}a_n\lambda^{-(2n+1)},\qquad a_0=\frac i2,\qquad a_{n+1}=\frac{2n+1}{2i}a_n.
$$

For example $a_1=1/4$, $a_2=-3i/8$, and $a_3=-15/16$. Repeated [integration by parts](../../../../../../integration-by-parts.md) bounds the remainder after any fixed number of terms by the order of the next term. Equivalently the [Fresnel tail expansion](../../../../../../fresnel-tail-expansion.md) is

$$
\begin{aligned}
P(\lambda)&\sim\sum_{m\ge0}\frac{(-1)^m(4m-1)!!}{2^{2m+1}\lambda^{4m+1}},\\
Q(\lambda)&\sim\sum_{m\ge0}\frac{(-1)^m(4m+1)!!}{2^{2m+2}\lambda^{4m+3}},\\
C(\lambda)&\sim A+P(\lambda)\sin\lambda^2-Q(\lambda)\cos\lambda^2,\\
S(\lambda)&\sim A-P(\lambda)\cos\lambda^2-Q(\lambda)\sin\lambda^2.
\end{aligned}
$$

Here $(-1)!!=1$. The first three terms of the requested cosine [Fresnel integral](../../../../../../fresnel-integral.md), counting its constant term, are

$$
\boxed{C(\lambda)=A+\frac{\sin\lambda^2}{2\lambda}-\frac{\cos\lambda^2}{4\lambda^3}+O(\lambda^{-5}).}
$$

For comparison, retaining one further correction in both [Finite Fresnel integrals](../../../../../../finite-fresnel-integrals.md) gives

$$
\begin{aligned}
C(\lambda)&=A+\frac{\sin\lambda^2}{2\lambda}-\frac{\cos\lambda^2}{4\lambda^3}-\frac{3\sin\lambda^2}{8\lambda^5}+O(\lambda^{-7}),\\
S(\lambda)&=A-\frac{\cos\lambda^2}{2\lambda}-\frac{\sin\lambda^2}{4\lambda^3}+\frac{3\cos\lambda^2}{8\lambda^5}+O(\lambda^{-7}).
\end{aligned}
$$

Unlike the small-argument [Taylor series](../../../../../../taylor-series.md), these large-argument [asymptotic expansions](../../../../../../asymptotic-expansion.md) must be truncated; adding indefinitely many terms at a fixed argument does not improve the approximation.

A calculator needs elementary arithmetic and its built-in sine and cosine, together with stored approximation coefficients. A convenient global construction uses [compactified approximation from endpoint asymptotics](../../../../../../compactified-approximation-from-endpoint-asymptotics.md). Define the exact real tail functions by

$$
Q+iP=e^{-i\lambda^2}\bigl(A(1+i)-C-iS\bigr),\qquad u=\frac{\lambda}{1+\lambda}.
$$

Then $P(0)=Q(0)=A$, while $P\sim1/(2\lambda)$ and $Q\sim1/(4\lambda^3)$ at infinity. Consequently

$$
p(u)=(1+\lambda)P(\lambda),\qquad q(u)=(1+\lambda)^3Q(\lambda)
$$

extend continuously to the compact interval $0\le u\le1$, with $p(1)=1/2$ and $q(1)=1/4$. Choose stored [polynomial approximations](../../../../../../polynomial-approximation.md) $p_N,q_N$ on that interval, constrained by the small-argument [Taylor series](../../../../../../taylor-series.md) and large-argument [asymptotic expansions](../../../../../../asymptotic-expansion.md), and calibrated across the intervening interval. The resulting elementary formula is

$$
\boxed{C_{\mathrm{calc}}(\lambda)=A+\frac{p_N(u)}{1+\lambda}\sin\lambda^2-\frac{q_N(u)}{(1+\lambda)^3}\cos\lambda^2.}
$$

Uniform errors $\delta_p,\delta_q$ in the stored [polynomial approximations](../../../../../../polynomial-approximation.md) give $|C_{\mathrm{calc}}-C|\le\delta_p+\delta_q$ for every positive argument. Existence of arbitrarily accurate such approximations follows from the [Weierstrass approximation theorem](../../../../../../weierstrass-approximation-theorem.md). A [Padé approximant](../../../../../../pade-approximant.md) with a denominator having no positive zero is an alternative implementation. Matching the two end expansions alone is not an error guarantee: the middle interval must also be controlled. For very small arguments, switching to the short [Taylor series](../../../../../../taylor-series.md) avoids cancellation. Ordinary finite-precision limitations in evaluating $\lambda^2$ and reducing its trigonometric phase remain those of the calculator itself.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
