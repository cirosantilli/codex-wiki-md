<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [joint probability density](../../../../../joint-probability-density.md) of the two [independent](../../../../../independent-random-variables.md) [standard normal random variables](../../../../../standard-normal-random-variable.md) is $(2\pi)^{-1}e^{-(x^2+y^2)/2}$. The [polar coordinates](../../../../../polar-coordinates.md) map has absolute [Jacobian determinant](../../../../../jacobian-determinant.md) $r$, so the [change of variables for probability densities](../../../../../change-of-variables-for-probability-densities.md) gives

$$
\boxed{f_{R,\Theta}(r,\theta)=\frac r{2\pi}e^{-r^2/2}
\mathbf1_{\{r>0,\ 0\leq\theta<2\pi\}}.}
$$

At the origin the angle may be assigned arbitrarily: that point has [probability](../../../../../probability.md) zero. The [joint probability density](../../../../../joint-probability-density.md) factorizes as a [Rayleigh distribution](../../../../../rayleigh-distribution.md) density $r e^{-r^2/2}$ and a [continuous uniform distribution](../../../../../continuous-uniform-distribution.md) density $1/(2\pi)$. Hence $R$ and $\Theta$ are [independent](../../../../../independent-random-variables.md).

For $u>0$, substitute $s=r^2/2$ to find

$$
\mathbb P(R^2\leq u)=\int_0^{\sqrt u}r e^{-r^2/2}\,dr
=\boxed{1-e^{-u/2}.}
$$

Therefore $R^2\sim\operatorname{Exp}(1/2)$, equivalently $\chi_2^2$, and applying a measurable function to $R$ preserves its [independence](../../../../../independent-random-variables.md) from $\Theta$. Explicitly, with $S=R^2$,

$$
\boxed{f_{\Theta,S}(\theta,s)=\frac1{4\pi}e^{-s/2}
\mathbf1_{\{0\leq\theta<2\pi,\ s>0\}}.}
$$

Thus $\Theta\sim\operatorname{Unif}[0,2\pi)$ and $S\sim\operatorname{Exp}(1/2)$ independently. This [polar decomposition of a planar standard normal vector](../../../../../polar-decomposition-of-a-planar-standard-normal-vector.md) separates the uniformly distributed direction from its random squared distance.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2015](../../../../2015-split.md)
5. [Past exam of the probability course of the University of Oxford](../../../../split.md)
6. [Probability course of the University of Oxford](../../../../../probability-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
