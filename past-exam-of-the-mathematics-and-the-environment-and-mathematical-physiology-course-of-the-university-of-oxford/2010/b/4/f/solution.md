<h1 id="b/4/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Write $c=c_1$, $\beta=(k_{-1}+k_1^+)/(k_1S_0)$ and $\kappa=k_1^+/(k_1S_0)$. Since $c_0=1-c$, the exact equations are

$$
\epsilon c_\tau=s-(s+\beta)c,\qquad s_\tau=-s+(s+\beta-\kappa)c.
$$

At the prescribed initial data $s=1,c=0$, $r_1=1$, rather than zero. The [quasi-steady-state approximation](../../../../../quasi-steady-state-approximation.md) would instead demand $c=s/(s+\beta)$, giving $c(0^+)=1/(1+\beta)$. This mismatch signals an [initial layer](../../../../../initial-layer.md).

Set $\sigma=\tau/\epsilon$ and expand $s=s_0+\epsilon s_1+\cdots$, $c=c_0+\cdots$. At leading order $s_0'=0$, so $s_0=1$, while $c_0'=1-(1+\beta)c_0$ and $c_0(0)=0$. Thus

$$
\boxed{s_{\rm in}=1+O(\epsilon),\qquad c_{\rm in}=\frac{1-e^{-(1+\beta)\sigma}}{1+\beta}+O(\epsilon).}
$$

For a more informative [substrate](../../../../../substrate-biochemistry.md) approximation, integration of $s_1'=-1+(1+\beta-\kappa)c_0$ with $s_1(0)=0$ gives

$$
s_{\rm in}=1-\epsilon\left[\frac{\kappa\sigma}{1+\beta}+\frac{1+\beta-\kappa}{(1+\beta)^2}(1-e^{-(1+\beta)\sigma})\right]+\cdots.
$$

On the slow scale $c_{\rm out}=s_{\rm out}/(s_{\rm out}+\beta)$ and $s_{{\rm out},\tau}=-\kappa s_{\rm out}/(s_{\rm out}+\beta)$, with matched leading value $s_{\rm out}(0)=1$. Integrating gives $s_{\rm out}+\beta\log s_{\rm out}=1-\kappa\tau$. In the overlap $1\ll\sigma\ll1/\epsilon$, the inner complex tends to $1/(1+\beta)$ and its [substrate](../../../../../substrate-biochemistry.md) slope matches the expansion of this [outer solution](../../../../../outer-expansion.md). A leading [composite asymptotic expansion](../../../../../additive-composite-expansion.md) is

$$
c_{\rm comp}(\tau)=\frac{s_{\rm out}(\tau)}{s_{\rm out}(\tau)+\beta}-\frac{e^{-(1+\beta)\tau/\epsilon}}{1+\beta},\qquad s_{\rm comp}=s_{\rm out}.
$$

It satisfies both initial values at leading order and smoothly joins the initial complex build-up to [substrate](../../../../../substrate-biochemistry.md) depletion. The displayed $O(\epsilon)$ inner [substrate](../../../../../substrate-biochemistry.md) term records the small binding-induced initial slip if greater accuracy is wanted.

## ↑ Ancestors (13)

1. [F](../f.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../split.md)
6. [Mathematics and the environment and mathematical physiology course of the University of Oxford](../../../../../mathematics-and-the-environment-and-mathematical-physiology-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
