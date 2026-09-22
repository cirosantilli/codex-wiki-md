<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Both alternatives can be made explicit. For a [conditional bias-corrected normal mean estimate](../../../../../../../conditional-bias-corrected-normal-mean-estimate.md), let $m$ be the observed pooled estimate and $w=n_1/n_2$, with $0<w<1$. Invert its conditional mean:

$$
\boxed{m=g(\widetilde\delta),\qquad
 g(d)=d+\frac{w}{\sqrt{I_1}}r(d\sqrt{I_1}-f_1).}
$$

This can be solved by bracketing or by Newton iteration $d_{k+1}=d_k-[g(d_k)-m]/g'(d_k)$. Since $r'(x)=-r(x)[x+r(x)]$,

$$
g'(d)=1-wr(x)[x+r(x)],\qquad x=d\sqrt{I_1}-f_1.
$$

The [variance](../../../../../../../variance-split.md) of a standard normal conditional on exceeding $-x$ is $1-r(x)[x+r(x)]$, strictly between zero and one. Positivity follows from nondegeneracy; the upper bound follows because the conditional mean $r(x)$ exceeds the truncation threshold $-x$. Hence $1-w<g'(d)<1$, so the equation has at most one root. As $d\to\infty$, $g(d)\sim d$; as $d\to-\infty$, the truncated stage-1 mean approaches its threshold and $g(d)\sim(1-w)d+wf_1/\sqrt{I_1}$, so a root exists for every finite $m$. Equivalently, differentiating the conditional [likelihood](../../../../../../../likelihood-function.md) divides the ordinary [likelihood](../../../../../../../likelihood-function.md) by $\Pr_d(C)$ and gives the same score equation. This conditional-[likelihood](../../../../../../../likelihood-function.md) correction is not exactly conditionally unbiased merely because it inverts a mean.

For an illustration, take $I_1=1$, $w=1/2$, $f_1=0$ and $m=0.5$. The equation is $d+\tfrac12\phi(d)/\Phi(d)=0.5$. Since $g(0)=0.39894$ and $g(0.5)\simeq0.75458$, the corrected estimate lies between zero and $0.5$; numerical solution gives **$\widetilde\delta\simeq0.14649$**, below the selected ordinary estimate.

For the [uniform minimum variance conditionally unbiased estimator](../../../../../../../uniform-minimum-variance-conditionally-unbiased-estimator.md), put $I_2=n_2/(2\sigma^2)$, $J=I_2-I_1>0$, $A=\widehat\delta_1$ and $V=\widehat\delta_2^*$. The fresh estimate $V$ is conditionally unbiased because it is independent of continuation. Let

$$
T=\frac{I_1A+JV}{I_2}=\widehat\delta_2,\qquad
c=\frac{f_1}{\sqrt{I_1}},\qquad
s^2=\frac1{I_1}-\frac1{I_2}=\frac{J}{I_1I_2}.
$$

Before selection, conditional Gaussian calculations give $A\mid T=t\sim N(t,s^2)$. Conditional on $C$ as well, this normal variable is truncated below $c$, so

$$
\mathbb E(A\mid T=t,C)=t+s\,r((t-c)/s).
$$

Using $V=(I_2T-I_1A)/J$, [Rao-Blackwellization](../../../../../../../rao-blackwellization.md) therefore gives

$$
\boxed{\widehat\delta_{\mathrm U}
=T-\frac{I_1s}{J}\,r\left(\frac{T-c}{s}\right).}
$$

Its conditional [expectation](../../../../../../../expected-value.md) is $\mathbb E[V\mid C]=\delta$, and its conditional [variance](../../../../../../../variance-split.md) cannot exceed that of $V$. To justify uniform minimum [variance](../../../../../../../variance-split.md), the joint conditional density of $(A,V)$ is a base density on $\{A\geq c\}$ multiplied by $\exp(\delta I_2T-\delta^2I_2/2)/\Pr_\delta(C)$. Thus $T$ is a [complete sufficient statistic](../../../../../../../complete-sufficient-statistic.md) in the one-parameter conditional [exponential family](../../../../../../../exponential-family-split.md), whose natural parameter ranges over an open real interval. The [Lehmann–Scheffé theorem](../../../../../../../lehmann-scheffe-theorem.md) proves the claim. The orthogonal pooled arm-average statistic is independent of the entire difference process and carries the nuisance common mean. Together with $T$, it gives a complete sufficient statistic in the selected two-parameter normal family, with an open natural-parameter space. Thus allowing that nuisance statistic does not improve the conditional unbiased estimate of the difference. For the same illustration, $I_2=2$, $J=1$ and $s=1/\sqrt2$ give **$\widehat\delta_{\mathrm U}\simeq0.21102$**. It differs from the conditional-[likelihood](../../../../../../../likelihood-function.md) estimate because exact conditional unbiasedness is a different criterion.

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
