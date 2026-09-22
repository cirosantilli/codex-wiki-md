<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**Non-characteristic.** The first-order [principal symbol](../../../../../../principal-symbol-of-a-partial-differential-equation.md) is $\nu_t-i\nu_x$, which equals one on $(0,1)$.

Set $z=x+it$. The equation is equivalent to $\partial_{\bar z}\phi=(\phi_x+i\phi_t)/2=0$. Because $\phi$ is continuously differentiable, the [Cauchy-Riemann equations](../../../../../../cauchy-riemann-equations.md) imply that it is a [holomorphic function](../../../../../../holomorphic-function.md) of $z$. Its convergent complex [Taylor series](../../../../../../taylor-series.md) restricts to a real [power series](../../../../../../power-series.md) along $t=0$, so $g$ is a [real analytic function](../../../../../../real-analytic-function.md).

For [smooth-data instability of the Cauchy-Riemann Cauchy problem](../../../../../../smooth-data-instability-of-the-cauchy-riemann-cauchy-problem.md), choose

$$
\boxed{\phi_n(x,t)=e^{-\sqrt n}\cos(n(x+it)).}
$$

These are [entire functions](../../../../../../entire-function.md) and satisfy the equation. Their initial [derivatives](../../../../../../derivative.md) obey $\sup_x|\partial_x^jg_n|\leq n^j e^{-\sqrt n}$, so every finite sum tends to zero. But

$$
\sup_{x\in\mathbb R}|\phi_n(x,t)|=e^{-\sqrt n}\cosh(n|t|)\longrightarrow\infty\qquad(t\ne0).
$$

Thus analytic solutions can exist while [continuous dependence on initial data](../../../../../../continuous-dependence-on-initial-data.md) fails for this smooth-data topology.

The [Cauchy estimate](../../../../../../cauchy-estimate.md) follows directly from the differentiated [Cauchy integral formula](../../../../../../cauchy-integral-formula.md):

$$
f^{(j)}(z_0)=\frac{j!}{2\pi i}\int_{|z-z_0|=r}\frac{f(z)}{(z-z_0)^{j+1}}\,dz,
\qquad
\boxed{|f^{(j)}(z_0)|\leq\frac{j!M}{r^j}.}
$$

The circle has length $2\pi r$, giving the bound for every integer $j\geq0$.

Put $w=\phi-\psi$ and integrate on the straight segment $z=\tau t/|t|$. For fixed $|x|<sR$, a disc centred at $x$ with radius approaching $R(\sigma(\tau)-s)$ stays inside $|\xi|\leq\sigma(\tau)R$. Applying the first-derivative [Cauchy estimate](../../../../../../cauchy-estimate.md) there gives

$$
|w_x(x,z)|\leq\frac{\sup_{|\xi|\leq\sigma(\tau)R,\;|\zeta|\leq\tau}|w(\xi,\zeta)|}{R(\sigma(\tau)-s)}.
$$

Integrating its modulus and taking the supremum over $|x|<sR$ is exactly the asserted integral estimate. The source cancels from $T\phi-T\psi$.

To obtain a [contraction mapping](../../../../../../contraction-mapping.md), use the [weighted holomorphic norm on a shrinking time domain](../../../../../../weighted-holomorphic-norm-on-a-shrinking-time-domain.md). Its finite-norm space consists of holomorphic functions on $\mathcal C_\alpha$ with zero initial value; the apparent quotient at $t=0$ is interpreted by a limit. Completeness follows because convergence in this norm implies [locally uniform convergence of holomorphic functions](../../../../../../locally-uniform-convergence-of-holomorphic-functions.md), including near $t=0$, and the limiting pointwise bounds give convergence in the norm.

Here is the explicit [contraction estimate on a shrinking holomorphic domain](../../../../../../contraction-estimate-on-a-shrinking-holomorphic-domain.md). Write $N=\|w\|_\alpha$, $r=|t|$, $A=\alpha(1-s)$, and choose

$$
\sigma(\tau)=s+\frac{A-\tau}{2\alpha}\qquad(0\leq\tau\leq r<A).
$$

Then $\sigma-s=(A-\tau)/(2\alpha)$ and $\alpha(1-\sigma)-\tau=(A-\tau)/2$. The whole auxiliary polydisc lies inside $\mathcal C_\alpha$, and its supremum of $|w|$ is at most $2N\tau/(A-\tau)$. Consequently

$$
\begin{aligned}
\frac{A-r}{r}|T\phi-T\psi|
&\leq\frac{4\alpha N}{R}\frac{A-r}{r}\int_0^r\frac{\tau}{(A-\tau)^2}\,d\tau\\
&=\frac{4\alpha N}{R}\left[1+\frac{A-r}{r}\log(1-r/A)\right]
\leq\frac{4\alpha N}{R}.
\end{aligned}
$$

Thus $\|T\phi-T\psi\|_\alpha\leq(4\alpha/R)\|\phi-\psi\|_\alpha$. Choose $0<\alpha<\min(\eta,R/4)$. The source is bounded on the closed polydisc, say by $M_f$, and $\|T0\|_\alpha\leq\alpha M_f$. Therefore $T$ maps the [Banach space](../../../../../../banach-space-split.md) into itself and is a strict [contraction mapping](../../../../../../contraction-mapping.md). The [Banach fixed-point theorem](../../../../../../contraction-mapping-theorem.md) gives a holomorphic fixed point with $\phi(x,0)=0$. Differentiating the integral identity yields $\phi_t-i\phi_x=f$, establishing this case of the [Cauchy-Kovalevskaya theorem](../../../../../../cauchy-kovalevskaya-theorem.md).

Finally, near each real initial point, a [real analytic function](../../../../../../real-analytic-function.md) $g$ has a holomorphic extension $G$. Apply the same construction to $\phi=G(x)+v$ with $v(x,0)=0$ and source $iG'(x)$, restricting the discs if necessary. This gives a local [real analytic function](../../../../../../real-analytic-function.md) of $(x,t)$ with the prescribed initial value. Equivalently the solution is $\boxed{\phi(x,t)=G(x+it)}$ wherever the extension is defined.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
