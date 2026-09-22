<h1 id="28i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A zero-cost stock holding $\theta$ has terminal payoff $\theta(S_1-1)$. If $a\le1$, shorting the share and holding a bond gives $1-S_1\ge0$ and a strictly positive payoff [almost surely](../../../../../../almost-sure-convergence.md). If $a>1$, both signs of $S_1-1$ occur with positive [probability](../../../../../../probability.md), so no nonzero holding is an arbitrage. Hence **arbitrage freedom is equivalent to $a>1$**.

The [equivalent martingale measures](../../../../../../risk-neutral-measure.md) are exactly the densities $Z(s)>0$ [almost everywhere](../../../../../../almost-everywhere.md) on $(0,a)$ satisfying

$$
\boxed{\frac1a\int_0^a Z(s)\,ds=1,\qquad\frac1a\int_0^a sZ(s)\,ds=1.}
$$

They exist for $a>1$: exponential tilts of the uniform law have means ranging continuously from zero to $a$, so one has mean one.

Under the usual utility assumptions $U'>0$, $U''<0$, and existence of an admissible optimum, $J(\theta)=E[U(w+\theta(S_1-1))]$ is [strictly concave](../../../../../../strictly-concave-function.md) and $J'(0)=U'(w)(a/2-1)$. Its decreasing derivative implies that the optimizer is positive exactly when $a>2$, negative when $a<2$, and zero when $a=2$, provided the feasible interval contains zero in its interior. The hypothesis $C^2$ alone is insufficient: a linear increasing utility can give an unbounded objective rather than a finite optimizer. Concavity and existence are implicit in the standard utility formulation.

For $a=2$, $\theta=0$ makes marginal utility constant, so the pricing [measure](../../../../../../measure.md) is the original uniform law and

$$
\boxed{p((S_1-1)^+)=\frac12\int_1^2(s-1)\,ds=\frac14.}
$$

For any equivalent pricing [measure](../../../../../../measure.md), the call [expectation](../../../../../../expected-value.md) is positive and strictly less than $E_QS_1/2=1/2$, since $(s-1)^+<s/2$ for $0<s<2$. Both endpoints can be approached. Symmetric densities concentrated in $[1-\delta,1+\delta]$ give prices tending to zero; symmetric densities concentrated near zero and two give prices tending to one half. Mix either density with an arbitrarily small amount of the uniform law to keep it everywhere positive; symmetry keeps its mean one. The set of positive mean-one densities is convex and the call price is linear, so every intermediate value is attained. Thus **the exact price range is $(0,1/2)$**, with neither endpoint attained.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28I](../../28i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
