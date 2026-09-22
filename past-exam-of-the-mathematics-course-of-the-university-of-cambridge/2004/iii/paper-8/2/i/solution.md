<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

First let $n\geq0$. The ordinary [Leibniz rule](../../../../../../leibniz-rule.md), applied to a test [function](../../../../../../function-split.md) $h$, gives

$$
\partial^n(fh)=\sum_{r=0}^n\binom nr f^{(r)}h^{(n-r)}.
$$

Equivalently, the composition of [differential operators](../../../../../../differential-operator.md) is

$$
\boxed{\partial^n m_f=\sum_{r=0}^n\binom nr m_{f^{(r)}}\partial^{n-r}.}
$$

For completeness, this formula follows by [induction](../../../../../../mathematical-induction.md): applying $\partial$ differentiates either the [coefficient](../../../../../../coefficient.md) or the remaining [derivative](../../../../../../derivative.md) of $h$, and the two contributions combine by $\binom nr+\binom n{r-1}=\binom{n+1}r$. The initial case is multiplication by $f$.

For all [integers](../../../../../../integer.md) $n$, define $\binom n0=1$ and $\binom nr=n(n-1)\cdots(n-r+1)/r!$. The [formal pseudodifferential composition rule](../../../../../../formal-pseudodifferential-composition-rule.md) is

$$
\boxed{\partial^n m_f=\sum_{r\geq0}\binom nr m_{f^{(r)}}\partial^{n-r},\qquad n\in\mathbb Z.}
$$

For $n=-s<0$, $\binom{-s}r=(-1)^r\binom{s+r-1}r$, so this is usually an infinite series. In particular

$$
\partial^{-1}m_f=m_f\partial^{-1}-m_{f'}\partial^{-2}+m_{f''}\partial^{-3}-\cdots.
$$

Applying $\partial$ on the left gives $m_f$: all later [coefficient](../../../../../../coefficient.md) [derivatives](../../../../../../derivative.md) cancel in pairs. This uniquely determines the normal-ordered inverse expansion. Repeating the inverse construction, or using the same binomial recurrence downward in $n$, gives every negative power. More explicitly, applying $\partial$ to the proposed $n$-series yields [coefficient](../../../../../../coefficient.md) $\binom nr+\binom n{r-1}=\binom{n+1}r$ at $f^{(r)}\partial^{n+1-r}$, so it is consistent with the already determined $(n+1)$-series. Negative powers here are formal; differentiation on all of $C^\infty(\mathbb R)$ has a nontrivial kernel and has no genuine two-sided inverse there.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
