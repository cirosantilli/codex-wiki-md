<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The [Lusternik-Schnirelmann-Borsuk theorem](../../../../../../lusternik-schnirelmann-theorem.md) has the following two equivalent covering formulations. For every integer $d\geq0$, a cover of the [sphere](../../../../../../sphere.md) $S^d$ by $d+1$ [closed sets](../../../../../../closed-set.md) has a member containing an [antipodal pair](../../../../../../antipodal-pair.md). The same assertion holds with [open sets](../../../../../../open-set.md) in place of [closed sets](../../../../../../closed-set.md). Thus **$d+1$ antipodal-pair-free open sets, or $d+1$ antipodal-pair-free closed sets, cannot cover $S^d$.** The dimension-zero case simply says that one set covering the two-point [sphere](../../../../../../sphere.md) contains both points.

Here is why the two versions agree. A finite [open cover](../../../../../../open-cover.md) of a [compact metric space](../../../../../../compact-metric-space.md) admits a [closed](../../../../../../closed-set.md) shrinking that still covers: sufficiently small [closed balls](../../../../../../closed-ball.md) subordinate to the [open cover](../../../../../../open-cover.md) can be grouped according to their containing open member. Applying the closed version to that shrinking proves the open version. Conversely, if a nonempty [closed](../../../../../../closed-set.md) subset $C$ of $S^d$ avoids [antipodal pairs](../../../../../../antipodal-pair.md), [compactness](../../../../../../compact-space.md) gives positive distance between $C$ and $-C$. A sufficiently small open neighbourhood of $C$ still avoids [antipodal pairs](../../../../../../antipodal-pair.md). Enlarge each member of a hypothetical closed counterexample in this way; the open version rules it out. Empty members cause no difficulty.

Another common equivalent formulation is the [Borsuk-Ulam theorem](../../../../../../borsuk-ulam-theorem.md): every [continuous](../../../../../../continuous-function.md) $f:S^d\to\mathbb R^d$ has $f(x)=f(-x)$ for some $x$, or, equivalently, every [continuous](../../../../../../continuous-function.md) [odd function](../../../../../../odd-function.md) $g:S^d\to\mathbb R^d$ has a zero. For example, if $d+1$ antipodal-pair-free [open sets](../../../../../../open-set.md) covered $S^d$, a subordinate [partition of unity](../../../../../../partition-of-unity.md) $(\phi_1,\ldots,\phi_{d+1})$ would give the [odd function](../../../../../../odd-function.md)

$$
g(x)=(\phi_i(x)-\phi_i(-x))_{i=1}^{d+1}
\in\{y\in\mathbb R^{d+1}:\textstyle\sum_i y_i=0\}\cong\mathbb R^d.
$$

It cannot vanish, since some $\phi_i(x)>0$, whereas antipodal-pair-freeness forces $\phi_i(-x)=0$. In the other direction, if an [odd function](../../../../../../odd-function.md) $g:S^d\to\mathbb R^d$ never vanishes, choose $d+1$ vectors $u_i$ forming a [regular simplex](../../../../../../regular-simplex.md) centred at the origin in $\mathbb R^d$. For $d\geq1$, the [open sets](../../../../../../open-set.md) $\{x:u_i\cdot g(x)>0\}$ cover $S^d$ and none contains an [antipodal pair](../../../../../../antipodal-pair.md), contradicting the covering theorem.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 13](../../../paper-13-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
