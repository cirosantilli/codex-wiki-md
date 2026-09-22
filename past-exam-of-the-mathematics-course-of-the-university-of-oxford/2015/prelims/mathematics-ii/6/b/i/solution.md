<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Fix $d$ strictly between $f'(a)$ and $f'(b)$, and set $F(x)=f(x)-dx$. The [function](../../../../../../../function-split.md) $F$ is [continuous](../../../../../../../continuous-function.md) on $[a,b]$: interior [differentiability](../../../../../../../differentiability.md) gives interior [continuity](../../../../../../../continuous-function.md), and the finite one-sided [derivatives](../../../../../../../derivative.md) give [continuity](../../../../../../../continuous-function.md) at the endpoints. The [extreme value theorem](../../../../../../../extreme-value-theorem.md) therefore gives a point $c$ where $F$ attains its [minimum](../../../../../../../minimum-of-a-subset-of-a-total-order.md).

Since $F'_+(a)=f'(a)-d<0$, for sufficiently small $h>0$ we have $F(a+h)<F(a)$, so $a$ cannot be a minimizing point. Since $F'_-(b)=f'(b)-d>0$, the quotient $(F(b-h)-F(b))/(-h)$ is positive for sufficiently small $h>0$, giving $F(b-h)<F(b)$. Thus $b$ cannot be a minimizing point either, and $c\in(a,b)$.

[Fermat's theorem on stationary points](../../../../../../../fermat-s-theorem-on-stationary-points.md) states that a [differentiable function](../../../../../../../differentiable-function.md) at an interior [local minimum](../../../../../../../local-minimum.md) or [local maximum](../../../../../../../local-maximum.md) has [derivative](../../../../../../../derivative.md) zero there. Applying it to $F$ gives

$$
\boxed{0=F'(c)=f'(c)-d,\qquad f'(c)=d.}
$$

This proves the relevant case of [Darboux's theorem](../../../../../../../darboux-s-theorem-analysis.md); the argument uses [continuity](../../../../../../../continuous-function.md) of $f$, with no assumption of [continuity](../../../../../../../continuous-function.md) of $f'$.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Mathematics II](../../../../mathematics-ii-split.md)
5. [Prelims](../../../../split.md)
6. [2015](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Oxford](../../../../../../split.md)
8. [Mathematics course of the University of Oxford](../../../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../../split.md)
