<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Write $a=\Lambda T$. The [deformation gradient](../../../../../deformation-gradient.md) of one interval of [shear flow](../../../../../shear-flow.md) is $S(a)=\begin{pmatrix}1&a\\0&1\end{pmatrix}$. An initial unit [material line](../../../../../material-curve.md) at angle $\theta$ therefore becomes $(\cos\theta+a\sin\theta,\sin\theta)$. Its orientation, including the correct quadrant, is

$$
\boxed{\theta_T=\operatorname{atan2}(\sin\theta,\cos\theta+a\sin\theta),\quad
\ell(\theta)=\sqrt{1+a\sin2\theta+a^2\sin^2\theta}.}
$$

For an unoriented line the angle is taken modulo $\pi$. If $\Lambda=0$, there is no [shear flow](../../../../../shear-flow.md): every $\lambda_N=1$ and $\mu=0$. The fluctuation and maximizing calculations below concern nonzero shear.

To quantify the [renovating shear flow](../../../../../renovating-shear-flow.md), use the intended isotropic model: each shear orientation is independent and uniform modulo $\pi$. Independence by itself does not specify a probability law and cannot fix the answer. Under the uniform law, conditional on every earlier deformation, the relative angle to the next shear is again uniform. Thus the logarithmic increments $\xi_n=\log\ell(\theta_n)$ are independent and identically distributed, even though the absolute orientation of the stretched [material line](../../../../../material-curve.md) need not be uniform. Since $\log\lambda_N=\sum_{n=1}^N\xi_n$, only the one-step angular mean is needed.

Write $\ell^2=A+B\cos(2\theta-\delta)$, where $A=1+a^2/2$, $B=|a|\sqrt{1+a^2/4}$ and $A^2-B^2=1$. The supplied angular logarithmic integral, with parameter $B/A$, gives

$$
r(a):=\langle\xi\rangle=\frac12\log\frac{A+\sqrt{A^2-B^2}}2
=\frac12\log(1+a^2/4).
$$

Therefore **the mean logarithmic stretching rate** is

$$
\boxed{\mu=\frac{\log(1+\Lambda^2T^2/4)}{2T}
=|\Lambda|\frac{\log(1+a^2/4)}{2|a|}.}
$$

This is the [mean logarithmic stretching in an isotropic renovating shear](../../../../../mean-logarithmic-stretching-in-an-isotropic-renovating-shear.md), and the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md) gives the same almost-sure [Lyapunov exponent](../../../../../lyapunov-exponent.md). Taking $\Lambda>0$ without loss for this statistic puts it in the requested form $\Lambda F(\Lambda T)$.

For $b=|\Lambda|T$, $F(b)=\log(1+b^2/4)/(2b)$. At small $b$, $\mu=\Lambda^2T/8+O(\Lambda^4T^3)$; at large $b$, $\mu\sim\log(b/2)/T$, tending to zero when $T$ increases at fixed shear rate. The maximizing nonzero $b$ solves

$$
\log z=2(1-z^{-1}),\qquad z=1+b^2/4.
$$

The difference $2(1-z^{-1})-\log z$ rises from zero up to $z=2$ and then strictly decreases to $-\infty$, so there is exactly one root beyond $2$. Numerically,

$$
\boxed{|\Lambda|T\simeq3.9605826,\qquad \mu_{\max}\simeq0.2012|\Lambda|.}
$$

Very rapid renovation gives little deformation per interval and cancels the first-order mean stretch. Long intervals provide strong deformation but progressively align a [material line](../../../../../material-curve.md) with the shear direction, so one interval stretches it only algebraically in $T$. Intermediate persistence combines substantial deformation with frequent reorientation, producing the finite maximum.

For the distribution, let $\gamma=\operatorname{arsinh}(|a|/2)$, so the singular stretches of $S(a)$ are $e^{\pm\gamma}$. In the right-singular-vector basis, $\ell^2=e^{2\gamma}\cos^2\varphi+e^{-2\gamma}\sin^2\varphi$. Put $q=\tanh\gamma=|a|/\sqrt{a^2+4}$. Factoring this expression and expanding its logarithm gives

$$
\xi=r(a)+\sum_{j=1}^{\infty}\frac{(-1)^{j+1}q^j}{j}\cos(2j\varphi),\qquad
v(a):=\operatorname{Var}\xi=\frac12\sum_{j=1}^{\infty}\frac{q^{2j}}{j^2}.
$$

The variance follows from angular orthogonality. These bounded independent increments imply

$$
\boxed{\frac{\log\lambda_N-Nr(a)}{\sqrt{Nv(a)}}\ \Longrightarrow\ N(0,1).}
$$

Accordingly the central part of the large-$N$ stretch distribution is approximately described by a [log-normal distribution](../../../../../log-normal-distribution.md), with density $[\lambda\sqrt{2\pi Nv}]^{-1}\exp[-(\log\lambda-Nr)^2/(2Nv)]$. This [central limit theorem](../../../../../central-limit-theorem.md) is not an assertion about arbitrarily extreme tails: the exact stretch has support inside $e^{-N\gamma}\leq\lambda_N\leq e^{N\gamma}$.

For $|a|\ll1$, the [log-stretch fluctuations in an isotropic renovating shear](../../../../../log-stretch-fluctuations-in-an-isotropic-renovating-shear.md) have

$$
r(a)=\frac{a^2}{8}-\frac{a^4}{64}+O(a^6),\qquad
v(a)=\frac{a^2}{8}-\frac{3a^4}{128}+O(a^6).
$$

To leading order the mean and variance of $\log\lambda_N$ both equal $Na^2/8$. Typical stretch is $\exp(Na^2/8)$, while its mean grows as $\exp(3Na^2/16)$. These moment statements can be justified directly rather than extrapolating the central Gaussian approximation: expansion of $\ell^p$ gives

$$
\langle\ell^p\rangle=1+\frac{p(p+2)}{16}a^2+O(a^4),\qquad
\boxed{\langle\lambda_N^p\rangle=\exp\left[\frac{Np(p+2)a^2}{16}+O(Na^4)\right]}
$$

for fixed $p$. In particular $\langle\lambda_N^2\rangle=(1+a^2/2)^N$ exactly. The leading small-$a$ log-normal approximation is especially precise in the many-small-renovations scaling with $Na^2$ fixed and $Na^4\to0$.

If the orientation law is not isotropic these formulas need not hold. For example, repeating a fixed shear direction gives $S(a)^N=S(Na)$, only algebraic stretch, and zero asymptotic logarithmic rate. The associated degenerate direction variables are independent, illustrating why the stated independence condition alone is insufficient to select the isotropic result.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 46](../../paper-46-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
