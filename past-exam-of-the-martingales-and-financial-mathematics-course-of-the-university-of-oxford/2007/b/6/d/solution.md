<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The [contingent claim payoff](../../../../../contingent-claim-payoff.md) derivative is $\Psi'(s)=2(s-K)_+$. Differentiating the [risk-neutral valuation](../../../../../risk-neutral-pricing.md) is justified by the finite [lognormal distribution](../../../../../log-normal-distribution.md), and $S_T$ is proportional to the starting stock value $s$. Thus

$$
\Delta(t,s)=\frac{2e^{-r\tau}}s
\mathbb E\bigl[(S_T^2-KS_T)\mathbf1_{\{S_T\geq K\}}\bigr],
\qquad\tau=T-t.
$$

For a [lognormal](../../../../../log-normal-distribution.md) terminal stock, completing the square in its Gaussian exponent gives

$$
\mathbb E[S_T^p\mathbf1_{\{S_T\geq K\}}]
=s^p e^{pr\tau+p(p-1)\sigma^2\tau/2}
\Phi\left(\frac{\log(s/K)+(r+(p-\tfrac12)\sigma^2)\tau}
{\sigma\sqrt\tau}\right).
$$

Use $p=2$ and $p=1$, and let $d_1=[\log(s/K)+(r+\sigma^2/2)\tau]/(\sigma\sqrt\tau)$. The result is

$$
\boxed{\Delta(t,s)=
2s e^{(r+\sigma^2)\tau}\Phi(d_1+\sigma\sqrt\tau)
-2K\Phi(d_1).}
$$

As $\tau\downarrow0$ this tends to $2(s-K)_+$, including value zero at $s=K$, as required. The extra $\sigma^2$ in the [option delta](../../../../../option-delta.md) PDE's stock drift gives the same shifted Gaussian arguments. This is [delta of a squared positive-part call](../../../../../delta-of-a-squared-positive-part-call.md).

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2007](../../../../2007-split.md)
5. [Past exam of the martingales and financial mathematics course of the University of Oxford](../../../../split.md)
6. [Martingales and financial mathematics course of the University of Oxford](../../../../../martingales-and-financial-mathematics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
