<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Cauchy point](../../../../../cauchy-point.md) minimizes the model along the negative [gradient](../../../../../gradient.md) ray inside the [trust region](../../../../../trust-region.md). With $q=g^THg$, write

$$
s_C=-\tau g,\qquad m(-tg)=a-t\|g\|^2+\tfrac12t^2q,\qquad 0\leq t\leq\Delta/\|g\|.
$$

If $q\leq0$, this last [quadratic function](../../../../../quadratic-function.md) decreases throughout the interval. If $q>0$, its unconstrained [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) occurs at $t=\|g\|^2/q$. Thus

$$
\boxed{\tau=\begin{cases}\Delta/\|g\|,&g^THg\leq0,\\\min\{\Delta/\|g\|,\|g\|^2/(g^THg)\},&g^THg>0.\end{cases}}
$$

The additive constant $a$ has no effect on the [Cauchy point](../../../../../cauchy-point.md). To obtain the [Cauchy decrease bound](../../../../../cauchy-decrease-bound.md), first suppose $q>0$. Since $\tau q\leq\|g\|^2$,

$$
a-m(s_C)=\tau\|g\|^2-\tfrac12\tau^2q\geq\tfrac12\tau\|g\|^2.
$$

The [spectral norm](../../../../../matrix-2-norm.md) inequality $q\leq\|H\|\|g\|^2$ gives $\tau\geq\min\{\Delta/\|g\|,1/\|H\|\}$. Hence

$$
\boxed{a-m(s_C)\geq\tfrac12\|g\|\min\{\Delta,\|g\|/\|H\|\}}.
$$

If $q\leq0$, the decrease is at least $\Delta\|g\|$, which also implies the displayed bound. When $H=0$, interpret $\|g\|/\|H\|=+\infty$. Thus the universal choice is $c=1/2$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the continuous optimisation course of the University of Oxford](../../../../split.md)
6. [Continuous optimisation course of the University of Oxford](../../../../../continuous-optimisation-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
