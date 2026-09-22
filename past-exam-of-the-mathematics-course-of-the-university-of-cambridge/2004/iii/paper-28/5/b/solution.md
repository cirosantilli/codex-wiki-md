<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Interpret the signed inverse-power force as $m\operatorname{sign}(x)/|x|^p$, so noninteger $p$ is meaningful on either side of the origin. Write $\alpha=1/p\in(0,2)$. Exactly as in part (a), the one-star [characteristic function](../../../../../../characteristic-function.md) is $1-I_{n,p}(t)/n$, where

$$
I_{n,p}(t)=\int_0^n\left(1-\cos\!\left(\frac{mt}{x^p}\right)\right)\,dx.
$$

The integrand is bounded near zero and is at most $m^2t^2/(2x^{2p})$ at infinity. The condition $2p>1$ thus makes its [integral](../../../../../../integral.md) finite. [Independence](../../../../../../independent-random-variables.md) and the [logarithm](../../../../../../logarithm.md) calculation in part (a) give the limiting [characteristic function](../../../../../../characteristic-function.md) $\exp(-I_p(t))$, with

$$
I_p(t)=\alpha m^\alpha|t|^\alpha J_\alpha,
\qquad J_\alpha=\int_0^\infty(1-\cos u)u^{-1-\alpha}\,du.
$$

Here we substituted $u=m|t|/x^p$. The [integral](../../../../../../integral.md) for $J_\alpha$ is finite because its integrand is $O(u^{1-\alpha})$ at zero and $O(u^{-1-\alpha})$ at infinity.

To determine the constant rather than leave it as an unevaluated [integral](../../../../../../integral.md), use the [Gamma function](../../../../../../gamma-function.md) representation

$$
u^{-1-\alpha}=\frac1{\Gamma(1+\alpha)}\int_0^\infty v^\alpha e^{-vu}\,dv.
$$

The integrand multiplied by $1-\cos u$ is nonnegative, so the [Tonelli theorem](../../../../../../tonelli-theorem.md) permits exchanging the [integrals](../../../../../../integral.md). For $v>0$ the inner [integral](../../../../../../integral.md) is

$$
\int_0^\infty e^{-vu}(1-\cos u)\,du
=\frac1v-\frac{v}{1+v^2}=\frac1{v(1+v^2)}.
$$

Consequently, substituting $z=v^2$ and using the [Euler beta function](../../../../../../beta-function.md) and [Gamma reflection formula](../../../../../../gamma-reflection-formula.md),

$$
\begin{aligned}
J_\alpha
&=\frac1{\Gamma(1+\alpha)}\int_0^\infty\frac{v^{\alpha-1}}{1+v^2}\,dv\\
&=\frac{\Gamma(\alpha/2)\Gamma(1-\alpha/2)}{2\Gamma(1+\alpha)}
=\frac{\pi}{2\Gamma(1+\alpha)\sin(\pi\alpha/2)}.
\end{aligned}
$$

Since $\Gamma(1+\alpha)=\alpha\Gamma(\alpha)$, this gives

$$
\boxed{c_p=\frac{\pi m^{1/p}}{2\Gamma(1/p)\sin(\pi/(2p))},\qquad
\phi(t)=e^{-c_p|t|^{1/p}}.}
$$

Every factor in $c_p$ is positive in the stated range. The [Lévy continuity theorem](../../../../../../levy-continuity-theorem.md) gives [weak convergence of random variables](../../../../../../convergence-in-distribution.md) because this [characteristic function](../../../../../../characteristic-function.md) is [continuous](../../../../../../continuous-function.md) at zero. The limit is strictly stable: if $Z_1,Z_2$ are [independent](../../../../../../independent-random-variables.md) copies of it, the [characteristic function](../../../../../../characteristic-function.md) of $aZ_1+bZ_2$ is

$$
\exp\{-c_p(|a|^\alpha+|b|^\alpha)|t|^\alpha\},
$$

which is the [characteristic function](../../../../../../characteristic-function.md) of $(|a|^\alpha+|b|^\alpha)^{1/\alpha}Z_1$. This proves the asserted index, as well as identifying the [symmetric stable distribution](../../../../../../symmetric-stable-distribution.md). In particular $p=2$ gives $c_2=\sqrt{\pi m/2}$, while $p=1$ gives $c_1=\pi m/2$, the centered [Cauchy distribution](../../../../../../cauchy-distribution.md) with that scale.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
