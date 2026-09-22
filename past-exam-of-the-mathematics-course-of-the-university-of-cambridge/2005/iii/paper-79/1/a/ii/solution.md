<h1 id="1/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There are two contributing regions: an endpoint of width $x^{-1}$ near $u=0$, and a very narrow peak near $u=1$. Both must be retained in the [asymptotic expansion](../../../../../../../asymptotic-expansion.md).

For the peak, set $a=e^{-x}$ and $u=1+av$. At fixed $v$, $\log u\sim av$ and $e^{-xu}\sim a$, so the integrand times $du$ approaches $dv/(1+v^2)$. This is the [Lorentzian contribution from shrinking regularization](../../../../../../../lorentzian-contribution-from-shrinking-regularization.md). Its total contribution is

$$
\int_{-\infty}^{\infty}\frac{dv}{1+v^2}=\pi.
$$

For example, cut off this region at $|u-1|=e^{-x/2}$: its scaled endpoints tend to infinity, while the changes in the exponential and logarithm inside the peak are exponentially small. The matched tails outside it are also exponentially small compared with the endpoint terms below.

At the endpoint, put $v=xu$ and $L=\log x$. To algebraic orders in $L^{-1}$, the regularizing denominator term is negligible there, giving the [Laplace endpoint expansion with a logarithmic denominator](../../../../../../../laplace-endpoint-expansion-with-a-logarithmic-denominator.md)

$$
\frac1x\int_0^\infty\frac{e^{-v}}{(L-\log v)^2}\,dv\sim\frac1{xL^2}\left[1+\frac2L\int_0^\infty e^{-v}\log v\,dv+\cdots\right].
$$

This integral represents the endpoint expansion only; it is cut off before the original peak when making the argument precise. Since $\Gamma'(1)=-\gamma_E$, with $\gamma_E$ the [Euler--Mascheroni constant](../../../../../../../euler-s-constant.md), the first two contributions to the original integral are

$$
\boxed{I(x)=\pi+\frac1{x(\log x)^2}+O\left(\frac1{x(\log x)^3}\right).}
$$

The endpoint correction refines to $[xL^2]^{-1}[1-2\gamma_E/L+3(\gamma_E^2+\pi^2/6)/L^2+\cdots]$, using [derivatives of the gamma function](../../../../../../../derivative-of-the-gamma-function.md). An application of [Watson's lemma](../../../../../../../watson-s-lemma.md) confined to $u=0$ would omit the leading peak contribution $\pi$.

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [1](../../../1.md)
4. [Paper 79](../../../../paper-79-split.md)
5. [Iii](../../../../split.md)
6. [2005](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
