<h1 id="1/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Taken literally, the printed condition is insufficient: the choice of which factor vanishes may depend on the multi-index. For a counterexample already at $m=2$, let $P=\partial_x^2$, let $\Omega=(0,a)\times(-b,b)$ be a small rectangle compactly contained in the unit ball, and choose $\chi\in C_c^\infty((-b,b))$ nonnegative with positive integral. Put

$$
u=x(a-x)\chi(y),\qquad v=1.
$$

On the vertical edges $u=0$, and on the horizontal edges $u$ and its [derivatives](../../../../../../../derivative.md) vanish. Every first [derivative](../../../../../../../derivative.md) of $v$ is zero. Thus for every $|\beta|\le1$ the same-index alternative in the PDF holds at every boundary point. But

$$
\boxed{\int_\Omega(Pu)v=-2a\int_{-b}^b\chi(y)\,dy\ne0=\int_\Omega u(P^*v).}
$$

The valid [complete boundary-jet condition for formal adjoints](../../../../../../../complete-boundary-jet-condition-for-formal-adjoints.md) is that, at each boundary point, either all [derivatives](../../../../../../../derivative.md) of $u$ through order $m-1$ vanish or all such [derivatives](../../../../../../../derivative.md) of $v$ vanish. On a bounded piecewise smooth domain with smooth coefficients up to its closure, repeated [integration by parts](../../../../../../../integration-by-parts.md) produces boundary terms of the form $(\partial^\gamma u)\partial^\delta(a_\alpha v)$, multiplied by a normal component, with $|\gamma|,|\delta|\le m-1$. Expanding the second factor shows that every summand vanishes under this stronger whole-jet alternative. Hence the desired identity holds under that condition. The later cap argument satisfies this stronger condition face by face, so it remains valid despite the literal error in this subpart. Boundary regularity and finite integrals are also needed for a general noncompact-support integration formula; the caps used below have them.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [1](../../../1.md)
4. [Paper 105](../../../../paper-105-split.md)
5. [Iii](../../../../split.md)
6. [2017](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
