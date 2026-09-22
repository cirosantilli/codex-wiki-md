<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $A_q=\langle f\rangle_{w,q}$ and $N_q=\|f\|_{w,q}$. The exponent on the finite-set expression is $-1/q'$ in the PDF; the TeX aid drops its prime. Ignore zero-measure sets, whose integrals vanish. The equivalence is

$$
\boxed{A_q\leq N_q\leq q'A_q,\qquad C_{1,q}=1,\quad C_{2,q}=q'=\frac q{q-1}.}
$$

For the first bound, let $E_a=\{|f|>a\}$ and choose a finite-measure subset $E\subset E_a$. Since $\int_E|f|\geq a|E|$,

$$
N_q\geq |E|^{-1/q'}\int_E|f|\geq a|E|^{1/q}.
$$

Exhaust $E_a$ by its intersections with bounded balls. If its measure is finite these give the desired bound $a|E_a|^{1/q}$ in the limit; if it is infinite they force $N_q=\infty$. Now take the supremum over $a$.

For the other direction it suffices to assume $0<A_q<\infty$; the zero and infinite cases are immediate. For a set $E$ with $0<|E|=m<\infty$, the [layer cake representation](../../../../../../layer-cake-representation.md) gives

$$
\int_E|f|=\int_0^\infty|E\cap E_t|\,dt\leq\int_0^\infty\min\{m,(A_q/t)^q\}\,dt.
$$

Split at $t_0=A_qm^{-1/q}$. The first contribution is $mt_0$, and the second is $A_q^qt_0^{1-q}/(q-1)$. Their sum is $q'A_qm^{1/q'}$. Multiply by $m^{-1/q'}$ and take the supremum. This proves the equivalence even when the quantities are extended-valued. The integral expression is an actual [norm](../../../../../../norm.md) on the [weak Lq space](../../../../../../weak-lq-space.md), since the [triangle inequality](../../../../../../triangle-inequality.md) holds inside every set integral. The distribution-function expression is generally a [quasi-norm](../../../../../../quasi-norm.md). The factor $q'$ is sharp: $f(x)=x^{-1/q}$ on $(0,\infty)$ has $A_q=1$ and attains $N_q=q'$ on every initial interval. In higher dimensions, multiply this example by the indicator of a unit box in the remaining coordinates.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
