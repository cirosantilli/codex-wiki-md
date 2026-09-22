<h1 id="b/6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a [continuous local martingale](../../../../continuous-local-martingale.md) $M$ starting at zero, [Burkholder-Davis-Gundy inequalities](../../../../burkholder-davis-gundy-inequalities.md) compare its maximal size with its quadratic-variation clock:

$$
c_p\,\mathbb E\langle M\rangle_T^{p/2}
\leq\mathbb E\sup_{t\leq T}|M_t|^p
\leq C_p\,\mathbb E\langle M\rangle_T^{p/2},\qquad p>0.
$$

They remain valid with infinite values, by stopping and passage to the limit. Their significance here is that the horizontal and vertical [martingales](../../../../martingale-split.md) share the same stopping-time clock, so one coordinate's maximum can determine moments of the other and of the clock. For a process started away from zero, first subtract its initial value.

Starting at $i$, the vertical coordinate starts at one and is stopped on first hitting zero. For $\lambda>1$, it reaches level $\lambda$ before zero with probability $1/\lambda$, by [optional stopping theorem](../../../../optional-sampling-theorem-for-a-supermartingale.md) of one-dimensional [Brownian motion](../../../../brownian-motion-split.md) on $[0,\lambda]$. Thus

$$
\boxed{\rho(\lambda)=
\begin{cases}1,&0<\lambda\leq1,\\1/\lambda,&\lambda>1.\end{cases}}
$$

The tail [integral](../../../../integral-split.md) formula gives

$$
\mathbb E(Y^*)^p=p\int_0^\infty \lambda^{p-1}\rho(\lambda)d\lambda
=\frac1{1-p}\quad(0<p<1),
$$

and it diverges for $p\geq1$.

The stopped [martingale](../../../../martingale-split.md) $Y_{t\wedge T_{\mathbb H}}-1$ has [quadratic variation](../../../../quadratic-variation.md) $t\wedge T_{\mathbb H}$. Its maximum in absolute value is $\max(1,Y^*-1)$, between $Y^*/2$ and $Y^*$, so it has precisely the same finite positive moments as $Y^*$. BDG therefore gives $\mathbb E T_{\mathbb H}^{p/2}<\infty$ exactly for $p<1$. Applying BDG to $X_{t\wedge T_{\mathbb H}}$, which starts at zero and has the same clock, yields

$$
\boxed{\mathbb E_i(X^*_{T_{\mathbb H}})^p<\infty\iff0<p<1,\qquad
\mathbb E_iT_{\mathbb H}^q<\infty\iff0<q<\tfrac12.}
$$

Taking the displayed $1/p$ or $1/q$ powers does not change finiteness. In particular the exit time is almost surely finite while its mean is infinite.

## ↑ Ancestors (12)

1. [6](../6.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../split.md)
5. [Stochastic differential equations and Brownian motion in complex analysis course of the University of Oxford](../../../../stochastic-differential-equations-and-brownian-motion-in-complex-analysis-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
