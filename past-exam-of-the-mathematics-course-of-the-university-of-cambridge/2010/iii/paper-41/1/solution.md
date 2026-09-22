<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [scaling hypothesis for critical phenomena](../../../../../scaling-hypothesis-for-critical-phenomena.md) says that the singular equilibrium [free-energy density](../../../../../free-energy-density.md) is a generalized homogeneous function of the thermal and field variables, after analytic backgrounds are removed. To derive the ordinary mean-field form, put $r=r_t t$, $u>0$ and neglect the higher powers near the transition. Rescale $m=\sqrt{r_t/u}\,|t|^{1/2}\psi$. Minimizing the quartic potential becomes

$$
A_s=\frac{r_t^2}{u}|t|^2\min_\psi\left[\frac{\operatorname{sgn}(t)}2\psi^2+\frac14\psi^4-\frac{\sqrt u}{r_t^{3/2}}\frac h{|t|^{3/2}}\psi\right].
$$

This is the [mean-field scalar free-energy scaling](../../../../../mean-field-scalar-free-energy-scaling.md) form with $a=r_t^2/u$, $b=\sqrt u/r_t^{3/2}$. The two functions correspond to $t>0$ and $t<0$; the latter has two pure-phase branches and a cusp at zero field. The question's $>$ and $<$ subscripts distinguish these temperatures above and below $T_c$.

Differentiating with respect to $h$ gives $m=-\partial_hA_s\propto|t|^{1/2}$ on an ordered pure branch, and differentiating again gives $\chi=-\partial_h^2A_s\propto|t|^{-1}$. Thus the displayed scaling form independently yields $\beta=1/2$ and $\gamma=1$.

To allow anomalous powers, replace it by

$$
A_s=a|t|^{2-\alpha}f_\pm\left(\frac{bh}{|t|^\Delta}\right).
$$

Then $\beta=2-\alpha-\Delta$ and $\gamma=2\Delta-(2-\alpha)$. Taking $t\to0$ at fixed small $h$ gives $A_s\propto|h|^{(2-\alpha)/\Delta}$, so $1/\delta=(2-\alpha-\Delta)/\Delta=\beta/\Delta$. Eliminating $\Delta$ proves the [Rushbrooke scaling relation](../../../../../rushbrooke-scaling-relation.md) and [Widom scaling relation](../../../../../widom-scaling-relation.md):

$$
\boxed{\alpha+2\beta+\gamma=2,\qquad\beta\delta=\Delta=\beta+\gamma.}
$$

These power-law relations assume the simple scaling form; marginal corrections or [dangerously irrelevant couplings](../../../../../dangerously-irrelevant-coupling.md) can require additional scaling variables.

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 41](../../paper-41-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
