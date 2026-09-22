<h1 id="10e/solution">Solution</h1>

↑ **Parent:** [10E](../10e.md)

The [Rolle theorem](../../../../../rolle-theorem.md) states that if a real function is continuous on $[u,v]$, differentiable on $(u,v)$, and has equal endpoint values, then its derivative vanishes somewhere in $(u,v)$. Order the $k$ distinct real roots as $r_1<\cdots<r_k$. The theorem gives a root of $f'$ in each interval $(r_j,r_{j+1})$. These intervals are disjoint, so the obtained roots are distinct:

$$
\boxed{f'\text{ has at least }k-1\text{ distinct real roots}.}
$$

We prove the requested bound for [positive roots of a polynomial](../../../../../positive-root-of-a-polynomial.md) by [mathematical induction](../../../../../mathematical-induction.md) on the number of nonzero terms. In fact, the proof also works with roots counted according to their [multiplicity](../../../../../multiplicity-mathematics.md). Write $V(p)$ for the number of sign changes and $N_+(p)$ for the positive-root count.

A one-term polynomial $a_1x^{d_1}$ has no positive roots and no sign changes. For the induction step, factor out the smallest power of $x$:

$$
q(x)=x^{-d_1}p(x)
=a_1+\sum_{j=2}^na_jx^{e_j},
\qquad e_j=d_j-d_1>0.
$$

For $x>0$ this factor is nonzero, so $N_+(q)=N_+(p)$, including multiplicities, and $V(q)=V(p)$. Differentiation removes exactly the constant term:

$$
q'(x)=\sum_{j=2}^ne_ja_jx^{e_j-1}.
$$

The exponents remain strictly increasing, and the positive multipliers $e_j$ do not change coefficient signs. The induction hypothesis therefore gives

$$
N_+(q')\le V(q'),\qquad
V(q')=V(a_2,\ldots,a_n).
$$

First suppose $a_1a_2<0$. Removing $a_1$ removes exactly one sign change, so $V(q)=V(q')+1$. If $q$ has positive roots $r_1<\cdots<r_k$ of multiplicities $m_1,\ldots,m_k$, its derivative has multiplicity $m_j-1$ at $r_j$ and, by the [Rolle theorem](../../../../../rolle-theorem.md), an additional root between each pair. Thus the [Rolle root count with multiplicities](../../../../../rolle-root-count-with-multiplicities.md) gives

$$
N_+(q')\ge\sum_{j=1}^k(m_j-1)+(k-1)=N_+(q)-1
$$

when there is a positive root. Consequently

$$
N_+(q)\le N_+(q')+1\le V(q')+1=V(q).
$$

If there is no positive root, the desired bound is automatic.

Now suppose $a_1a_2>0$, so $V(q)=V(q')$. Again the zero-root case is immediate. Otherwise, multiplying $q$ by $-1$ if necessary lets us assume $a_1>0$ and $a_2>0$ without changing roots or sign changes. For sufficiently small $x>0$,

$$
q(x)>0,\qquad q'(x)>0,
$$

since $q(0)=a_1$ and the lowest-power term of $q'$ has positive coefficient. Choose such a point $u$ before the first positive root $r_1$. The [mean value theorem](../../../../../mean-value-theorem.md) on $[u,r_1]$ gives a point $v\in(u,r_1)$ with

$$
q'(v)=\frac{q(r_1)-q(u)}{r_1-u}<0.
$$

But $q'(u)>0$. The [intermediate value theorem](../../../../../intermediate-value-theorem.md) applied to the polynomial $q'$ therefore gives an extra root in $(u,v)$, before $r_1$. It is distinct from the roots at $r_j$ and those between consecutive roots. Hence

$$
N_+(q')\ge N_+(q),
\qquad
N_+(q)\le N_+(q')\le V(q')=V(q).
$$

Both sign cases complete the induction:

$$
\boxed{N_+(p)\le V(p).}
$$

**An initial sign change allows one extra positive root; without that sign change, the derivative must already turn before the first positive root.** This is the upper-bound part of the [Descartes' rule of signs](../../../../../descartes-rule-of-signs.md). The multiplicity claim used above follows by differentiating $q(x)=(x-r)^mh(x)$ with $h(r)\ne0$: the derivative has a factor $(x-r)^{m-1}$ and its remaining factor is nonzero at $r$.

## ↑ Ancestors (10)

1. [10E](../10e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ia](../../split.md)
4. [2016](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
