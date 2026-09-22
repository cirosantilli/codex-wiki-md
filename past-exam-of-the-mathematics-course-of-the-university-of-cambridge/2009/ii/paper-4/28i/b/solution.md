<h1 id="28i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The fixed terminal height makes $-y(T)+T=T-1$, so this is a minimum-time problem. An optimal path can be taken entirely in $y\ge1/2$. To justify the positive-$y$ calculation despite the absolute value in the dynamics, the time of a spatial path is its length in the metric $ds/\sqrt{|y|}$. Reflection to $|y|$ preserves this time; clipping the reflected height below $1/2$ to $1/2$ leaves the endpoints unchanged and cannot increase time, since it decreases vertical length and increases the speed available. Any excursion below $1/2$ strictly wastes time. Thus an optimum does not meet $y=0$.

Use $H=\sqrt y(pu+qv)-1$. Its maximum is $\sqrt y\sqrt{p^2+q^2}-1$, attained at

$$
u=\frac p{\sqrt{p^2+q^2}},\qquad v=\frac q{\sqrt{p^2+q^2}}.
$$

The [costate](../../../../../../costate.md) equations and [free-terminal-time transversality condition](../../../../../../free-terminal-time-transversality-condition.md) give

$$
\dot p=0,\qquad\dot q=-\frac{\sqrt{p^2+q^2}}{2\sqrt y},\qquad
\sqrt y\sqrt{p^2+q^2}=1.
$$

The last identity holds throughout because the maximized autonomous [Hamiltonian](../../../../../../hamiltonian.md) is constant. An abnormal extremal would instead have maximized [Hamiltonian](../../../../../../hamiltonian.md) $\sqrt y\sqrt{p^2+q^2}=0$, forcing both [costates](../../../../../../costate.md) to vanish and contradicting their nontriviality. Thus the normal choice is valid. Also $p\ne0$, since otherwise $x$ cannot reach one; in fact $p>0$ because $\dot x$ has its constant sign.

Now express both requested derivatives using the [costates](../../../../../../costate.md):

$$
\frac{dy}{dx}=\frac qp,\qquad
\frac{d^2y}{dx^2}=\frac{\dot q}{p\dot x}
=-\frac{p^2+q^2}{2yp^2}.
$$

Consequently the optimal trajectory satisfies

$$
\boxed{1+\left(\frac{dy}{dx}\right)^2+2y\frac{d^2y}{dx^2}=0.}
$$

The maximizing controls above and the fixed endpoints determine the relevant extremal; the displayed equation is the requested necessary trajectory equation.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28I](../../28i.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
