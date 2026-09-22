<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For $s\geq0$ and $\xi\in\mathbb R$, define the [characteristic curve](../../../../../../characteristic-curve.md) $X(t;s,\xi)$ by

$$
\dot X(t;s,\xi)=F(t,X(t;s,\xi)),
\qquad
X(s;s,\xi)=\xi.
$$

The bounded derivative $F_x$ makes $F(t,\cdot)$ globally [Lipschitz](../../../../../../lipschitz-continuity.md), uniformly in $t$. On each finite time interval, $|F(t,x)|\leq|F(t,0)|+L|x|$, so [Gronwall inequality](../../../../../../gronwall-inequality.md) prevents finite-time escape. The [Picard-Lindelöf theorem](../../../../../../picard-lindelof-theorem.md) therefore gives a unique trajectory for every finite $t\geq0$. Differentiation in $\xi$ gives

$$
\partial_\xi X(t;s,\xi)
=\exp\left(\int_s^tF_x(r,X(r;s,\xi))\,dr\right)>0,
$$

so the [characteristic flow map](../../../../../../characteristic-flow-map.md) is a $C^1$ increasing diffeomorphism.

Along a characteristic, the [chain rule](../../../../../../chain-rule.md) changes the equation into

$$
\frac d{dt}u(t,X(t;0,\xi))=g(t,X(t;0,\xi)).
$$

Tracing $(t,x)$ backward by the flow therefore gives

$$
u(t,x)=u_0(X(0;t,x))+\int_0^tg(s,X(s;t,x))\,ds.
$$

The regularity of the flow makes this a $C^1$ [classical solution](../../../../../../classical-solution.md). Conversely, every classical solution obeys the same ordinary differential equation along every characteristic, so the formula also proves uniqueness.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
