<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

**The joint generator.** With $\theta$ again measured in dollars, [portfolio wealth](../../../../../portfolio-wealth.md) obeys

$$
dw=\sigma(x)\theta\,dW+[rw+(\mu(x)-r)\theta-c]\,dt.
$$

Its noise and the factor noise are driven by the same [Brownian motion](../../../../../brownian-motion-split.md). Their [quadratic covariation](../../../../../quadratic-covariation.md) is $\sigma(x)\theta\alpha(x)\,dt$, so the [diffusion generator](../../../../../diffusion-generator.md) has a cross derivative. [Dynamic programming](../../../../../dynamic-programming.md) and the [Itô formula](../../../../../ito-s-lemma.md) give

$$
\boxed{\begin{aligned}
0={}&\tfrac12\alpha^2V_{xx}+\beta V_x-\rho V+rwV_w\\
&+\sup_{\theta\in\mathbb R}
\left\{(\mu-r)\theta V_w+\sigma\alpha\theta V_{wx}
+\tfrac12\sigma^2\theta^2V_{ww}\right\}
+\sup_{c\geq0}\{U(c)-cV_w\}.
\end{aligned}}
$$

All coefficient functions in this formula are evaluated at $x$. The cross derivative is essential: it gives [intertemporal hedging demand](../../../../../intertemporal-hedging-demand.md). Normalizing [CRRA utility](../../../../../constant-relative-risk-aversion-utility.md) as $U(c)=c^p/p$, where $p=1-R$, the two optimizations give, at nonzero volatility,

$$
c^*=(V_w)^{-1/R},\qquad
\theta^*=-\frac{(\mu-r)V_w+\sigma\alpha V_{wx}}{\sigma^2V_{ww}},
$$

and hence

$$
0=\tfrac12\alpha^2V_{xx}+\beta V_x-\rho V+rwV_w
-\frac{[(\mu-r)V_w+\sigma\alpha V_{wx}]^2}{2\sigma^2V_{ww}}
+\frac R p(V_w)^{p(-1/R)}.
$$

Here $p(-1/R)=1-1/R$.

**Homogeneity and the reduced equation.** Scaling initial [portfolio wealth](../../../../../portfolio-wealth.md) and both controls preserves the [portfolio wealth](../../../../../portfolio-wealth.md) constraint and multiplies the objective by the positive number $b^p$. Thus

$$
V(w,x)=\frac{w^p}{p}f(x),\qquad f(x)>0.
$$

This expression is valid for both signs of $p$: $V$ is negative when $R>1$, but its [portfolio wealth](../../../../../portfolio-wealth.md) derivative is positive. Its derivatives are

$$
V_w=w^{-R}f,\quad V_{ww}=-Rw^{-R-1}f,\quad
V_{wx}=w^{-R}f',\quad
V_x=\frac{w^p}{p}f',\quad V_{xx}=\frac{w^p}{p}f''.
$$

Substitution yields

$$
\boxed{
\tfrac12\alpha^2f''+\beta f'+(pr-\rho)f
+\frac{p[(\mu-r)f+\sigma\alpha f']^2}{2R\sigma^2f}
+R f^{(R-1)/R}=0.}
$$

The resulting feedback is

$$
\boxed{\frac{c^*}{w}=f^{-1/R},\qquad
\frac{\theta^*}{w}=\frac{\mu-r}{R\sigma^2}
+\frac{\alpha}{R\sigma}\frac{f'}f.}
$$

The first portfolio term is myopic, and the second is [intertemporal hedging demand](../../../../../intertemporal-hedging-demand.md).

**Constant market price of risk.** If $\mu-r=\sigma\kappa$ and volatility is nonzero, the portfolio term becomes $p(\kappa f+\alpha f')^2/(2Rf)$, so the magnitude of stock volatility disappears. Applying the [power transformation of a complete-market investment equation](../../../../../power-transformation-of-a-complete-market-investment-equation.md) $f=g^R$ cancels the squared-gradient terms and gives the further reduction

$$
\boxed{\tfrac12\alpha^2g''+
\left(\beta+\frac{p\kappa\alpha}{R}\right)g'
-\gamma_M g+1=0,\qquad
\gamma_M=\frac{\rho-p(r+\kappa^2/(2R))}{R}.}
$$

For $\gamma_M>0$ its economic solution is $g=1/\gamma_M$. Thus

$$
\boxed{V(w,x)=\frac{\gamma_M^{-R}w^p}{p},\qquad
c^*=\gamma_M w,\qquad
\theta^*=\frac{\kappa w}{R\sigma(x)}.}
$$

To see why this solves the [investment-consumption problem](../../../../../investment-consumption-problem.md), optimize directly over [Brownian portfolio exposures](../../../../../brownian-portfolio-exposures.md), writing $y=\sigma(x)\theta$. The [portfolio wealth](../../../../../portfolio-wealth.md) equation becomes $dw=y\,dW+(rw+\kappa y-c)dt$, which no longer contains $X$. With nonzero volatility the same admissible exposure processes are available for every factor state, so the attainable wealth-consumption pairs, and therefore the value, are exactly those of the [Merton consumption-investment problem](../../../../../merton-consumption-investment-problem.md). This also excludes extraneous solutions of the linear equation without imposing artificial factor boundary data.

The printed boundedness assumptions do not ensure nonzero volatility or a finite value. The unsimplified [HJB equation](../../../../../hamilton-jacobi-bellman-equation.md) remains the correct control equation at a zero of $\sigma$. There the hedge term vanishes; if $\mu\ne r$, the riskless excess return gives [arbitrage](../../../../../arbitrage.md) with unrestricted holdings. Under $\mu-r=\sigma\kappa$, a zero-volatility state offers only the bank exposure at that instant. For example $\sigma\equiv0$, $\mu\equiv r$ satisfies this relation for any chosen $\kappa$, but its value uses $\gamma_0=[\rho-pr]/R$, not a fictitious nonzero risk premium. **The constant-value formula using $\kappa$ presupposes access to the Brownian exposure**, with sufficient integrability for the corresponding holdings. Additive utility constants again only shift $V$ by a constant divided by $\rho$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 40](../../paper-40-split.md)
3. [Iii](../../split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
