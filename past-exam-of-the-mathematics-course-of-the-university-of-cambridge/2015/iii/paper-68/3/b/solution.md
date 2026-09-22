<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First let $L$ be a [bounded linear operator](../../../../../../continuous-linear-operator.md) on $H$ satisfying the symmetric positive-definiteness convention in part (a). For any direction $w\in H$, expansion of the quadratic functional gives

$$
\begin{aligned}
 I(v+\varepsilon w)-I(v)
 &=2\varepsilon\{\langle Lv,w\rangle-\langle f,w\rangle\}
   +\varepsilon^2\langle Lw,w\rangle,\\
 DI(v)[w]&=2\langle Lv-f,w\rangle.
\end{aligned}
$$

Thus vanishing of the [first variation](../../../../../../first-variation.md) in every direction is precisely the weak equation $\langle Lu,w\rangle=\langle f,w\rangle$ for every $w$. In this whole-space bounded-operator setting it is equivalent to $Lu=f$, the [Euler-Lagrange equation](../../../../../../euler-lagrange-equation.md).

If $u$ solves that equation, set $v=u+w$. The linear terms cancel:

$$
\boxed{I(v)-I(u)=\langle L(v-u),v-u\rangle\geq0,}
$$

with equality only when $v=u$. Hence **the weak solution is the unique global minimizer**. Conversely, any minimizer has zero [first variation](../../../../../../first-variation.md), and therefore solves the weak equation. For a symmetric [bounded bilinear form](../../../../../../bounded-bilinear-form.md) $B$ on a form space $V$, exactly the same calculation gives $I(v)=B(v,v)-2\ell(v)$ and $B(u,w)=\ell(w)$ for every $w\in V$; it does not require an unbounded differential operator to map every $v\in V$ into $H$.

Existence for every $f$ requires an extra hypothesis if “positive definite” means only strict positivity. The [coercive operator](../../../../../../coercive-operator.md) bound makes the form coercive, so the [Lax-Milgram theorem](../../../../../../lax-milgram-theorem.md) supplies existence and uniqueness. Without that bound, the [diagonal operator on sequence space](../../../../../../diagonal-operator-on-sequence-space.md) $L(x_n)=(x_n/n)$ on $\ell^2$ is symmetric and strictly positive, but $f=(1/n)$ belongs to $\ell^2$ and its formal inverse $(1,1,\ldots)$ does not. Thus strict positivity alone proves uniqueness and the minimizing property of a solution when one exists, not existence for all $f$.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [Section A](../../section-a.md)
4. [Paper 68](../../../paper-68-split.md)
5. [Iii](../../../split.md)
6. [2015](../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../split.md)
