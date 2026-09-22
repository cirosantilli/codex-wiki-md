<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For a nonconstant [rational map](../../../../../rational-map-complex-analysis.md), choose local holomorphic coordinates $u$ at $p$ and $v$ at $R(p)$, both vanishing at their centres. Its local expression has the form

$$
v\circ R\circ u^{-1}(t)=a t^e+O(t^{e+1}),\qquad a\ne0.
$$

The [local degree of a holomorphic map](../../../../../local-degree-of-a-holomorphic-map.md) is $e$. A [critical point of a rational map](../../../../../critical-point-of-a-rational-map.md) is one with $e\geq2$, and its [critical multiplicity](../../../../../critical-multiplicity-of-a-rational-map.md) is $e-1$. Both are unchanged by coordinate changes with nonzero first [derivatives](../../../../../derivative.md). At finite points where $R$ is finite, multiplicity is the [derivative](../../../../../derivative.md)'s zero order; at [poles](../../../../../pole.md) and infinity it must be computed in the corresponding reciprocal coordinate.

We give an algebraic proof of the total count. Local [derivatives](../../../../../derivative.md) are holomorphic and not identically zero, so their zeros are isolated; [compactness](../../../../../compact-space.md) makes the sphere critical set finite. Choose a regular target value and make it infinity by a target [Möbius transformation](../../../../../mobius-transformation.md). There are then $d$ simple [poles](../../../../../pole.md). Independently choose a noncritical source point not mapping to this value and make it source infinity. In these coordinates all [poles](../../../../../pole.md) are finite and simple, and infinity is a regular point with finite image. Write the resulting map as $P/Q$, where $P,Q$ are coprime, $\deg Q=d$, and $\deg P\leq d$. Regularity at infinity gives

$$
R(z)=a+\frac b z+O(z^{-2}),\quad b\ne0,\qquad R'(z)=-\frac b{z^2}+O(z^{-3}).
$$

Since $R'=(P'Q-PQ')/Q^2$, its numerator $W=P'Q-PQ'$ therefore has degree exactly $2d-2$. At every [pole](../../../../../pole.md) $p$, $W(p)=-P(p)Q'(p)\ne0$, so the roots of $W$ are precisely the finite [rational critical points](../../../../../critical-point-of-a-rational-map.md), with their [critical multiplicities](../../../../../critical-multiplicity-of-a-rational-map.md). Infinity was chosen regular. The [fundamental theorem of algebra](../../../../../fundamental-theorem-of-algebra.md) now proves

$$
\boxed{\sum_{p\in\widehat{\mathbb C}}(e_p(R)-1)=2d-2.}
$$

The coordinate changes preserve the [local degrees of a holomorphic map](../../../../../local-degree-of-a-holomorphic-map.md), so this is the count for the original map. The printed critical-point count is **with multiplicity**: for example $z^d$ has only two distinct [rational critical points](../../../../../critical-point-of-a-rational-map.md), zero and infinity, each of multiplicity $d-1$.

[Local degrees of a holomorphic map](../../../../../local-degree-of-a-holomorphic-map.md) multiply under composition, since substituting leading powers of orders $e$ and $f$ gives order $ef$. Thus

$$
e_p(P^n)=\prod_{j=0}^{n-1}e_{P^j(p)}(P),\qquad\boxed{\operatorname{Crit}(P^n)=\bigcup_{j=0}^{n-1}P^{-j}(\operatorname{Crit}(P)).}
$$

If $p$ is critical for $P$, the first factor is at least two, so it is critical for every positive iterate. Conversely a product of positive integers can exceed one only if one factor exceeds one, so a [rational critical point](../../../../../critical-point-of-a-rational-map.md) of $P^n$ reaches a [rational critical point](../../../../../critical-point-of-a-rational-map.md) of $P$ in some $j<n$ steps (including $j=0$). At finite points this is also the [derivative](../../../../../derivative.md) [chain rule](../../../../../chain-rule.md) $(P^n)'(z)=\prod_{j=0}^{n-1}P'(P^j(z))$; the local-degree argument covers infinity as well. This proves both assertions about [critical points of iterates of a rational map](../../../../../critical-points-of-iterates-of-a-rational-map.md).

For the given [polynomial](../../../../../polynomial-split.md) the finite [derivative](../../../../../derivative.md) is $2z$, so the only finite [rational critical point](../../../../../critical-point-of-a-rational-map.md) is zero. Its orbit is

$$
0\longmapsto i\longmapsto-1+i\longmapsto-i\longmapsto-1+i.
$$

The last two points form an exact two-cycle, whose [periodic-orbit multiplier](../../../../../multiplier-of-a-periodic-orbit-of-an-iteration.md) is

$$
\lambda=P'(-1+i)P'(-i)=4(-1+i)(-i)=4(1+i),\qquad|\lambda|=4\sqrt2>1.
$$

Thus $a=-1+i$ is a [repelling periodic point](../../../../../repelling-periodic-point.md). To justify its Julia membership directly, suppose the iterates were normal near $a$. A [subsequence](../../../../../subsequence.md) of $(P^2)^n$, all fixing $a$, would converge spherically on a neighborhood. Its limit takes the finite value $a$ there, so in a smaller neighborhood it and the tail of that [subsequence](../../../../../subsequence.md) lie in a finite coordinate chart. The [Cauchy integral formula](../../../../../cauchy-integral-formula.md) then bounds the [derivatives](../../../../../derivative.md) at $a$. But those [derivatives](../../../../../derivative.md) equal $\lambda^n$, unbounded, a contradiction. Therefore $a\in J(P)$. Complete backward invariance of the [Julia set](../../../../../julia-set.md) and $P^2(0)=a$ give

$$
\boxed{0\in J(z^2+i).}
$$

The [critical orbit](../../../../../critical-orbit-of-a-rational-map.md) is bounded but preperiodic to a repelling [holomorphic cycle](../../../../../cycle-of-a-holomorphic-map.md), illustrating that boundedness alone does not put a point in the [Fatou set](../../../../../fatou-set.md).

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
