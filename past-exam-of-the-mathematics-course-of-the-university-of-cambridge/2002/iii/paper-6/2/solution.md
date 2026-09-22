<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Use the dominated form of the real [Hahn-Banach theorem](../../../../../hahn-banach-theorem.md). Let $p:V\to\mathbb R$ be a [sublinear functional](../../../../../sublinear-function.md) on a real [vector space](../../../../../vector-space-split.md), meaning $p(x+y)\le p(x)+p(y)$ and $p(tx)=tp(x)$ for $t\ge0$. If a [linear functional](../../../../../linear-functional.md) $f$ on a [vector subspace](../../../../../vector-subspace.md) $M$ satisfies $f\le p$ there, then it has a linear extension $F$ to $V$ with $F\le p$ everywhere.

Here is the one-dimensional extension step. For $z\notin M$, the value $a=F(z)$ must satisfy

$$
\sup_{m\in M}\{f(m)-p(m-z)\}\le a\le\inf_{m\in M}\{p(m+z)-f(m)\}.
$$

This interval is nonempty: for any $m,n\in M$,

$$
f(m)+f(n)=f(m+n)\le p(m+n)\le p(m-z)+p(n+z),
$$

so every candidate lower bound is at most every candidate upper bound. The candidates with $m=n=0$ also bound the endpoints by finite numbers, so a real $a$ can be chosen. Define $F(m+tz)=f(m)+ta$. For $t>0$, the upper bound, applied to $m/t$, gives $F(m+tz)\le p(m+tz)$ after multiplication by $t$. For $t<0$, the lower bound applied to $m/(-t)$ gives the same conclusion after multiplication by $-t$; $t=0$ is the original hypothesis. Thus the extension remains dominated.

Order all dominated extensions by extension of their domains and values. Every chain has the dominated linear union as an upper bound. The [Zorn lemma](../../../../../zorn-s-lemma.md) supplies a maximal extension. If its domain were not all of $V$, the step just proved would enlarge it, a contradiction. **This proves the real Hahn-Banach extension theorem.** In particular, taking $p(x)=\|f\|\|x\|$ on a [normed vector space](../../../../../normed-vector-space.md) and applying the domination to both $x$ and $-x$ yields the usual norm-preserving extension of a [bounded linear functional](../../../../../continuous-linear-functional.md).

For [generalized limits](../../../../../generalized-limit.md), take $V=\ell^\infty(\mathbb N;\mathbb R)$, the [l-infinity sequence space](../../../../../l-infinity-sequence-space.md), and $M=c$, the [convergent sequence space](../../../../../convergent-sequence-space.md). Let $f(x)=\lim_nx_n$ on $c$ and $p(x)=\limsup_nx_n$ on $V$. This $p$ is finite and sublinear, and agrees with $f$ on $c$. The dominated extension $L$ therefore satisfies

$$
L(x)\le\limsup_nx_n,\qquad -L(x)=L(-x)\le-\liminf_nx_n.
$$

Thus **a generalized limit exists**, with

$$
\boxed{\liminf_nx_n\le L(x)\le\limsup_nx_n.}
$$

It is positive, agrees with the ordinary limit on every [convergent sequence](../../../../../convergent-sequence.md), and satisfies $|L(x)|\le\|x\|_\infty$. Since $L(\mathbf1)=1$, its [operator norm](../../../../../operator-norm.md) is exactly one.

If generalized limits are additionally required to be shift invariant, the same theorem gives the stronger [Banach limit](../../../../../banach-limit.md). Replace the dominating functional by

$$
p_C(x)=\limsup_{N\to\infty}\frac1N\sum_{j=1}^Nx_j.
$$

It is again sublinear and agrees with $f$ on $c$, by the [Cesaro theorem for convergent sequences](../../../../../cesaro-theorem-for-convergent-sequences.md). The resulting $L_C$ lies between the lower and upper limits of the [Cesaro means](../../../../../cesaro-mean.md). These in turn lie between the ordinary lower and upper limits of a bounded sequence, so $L_C$ is a positive, norm-one extension of the ordinary limit. For the [left shift on bounded sequences](../../../../../left-shift-on-bounded-sequences.md) $S$, the means of $Sx-x$ equal $(x_{N+1}-x_1)/N\to0$. Applying domination to both signs forces $L_C(Sx-x)=0$. Hence

$$
\boxed{L_C(Sx)=L_C(x).}
$$

This [Cesàro construction of a Banach limit](../../../../../cesaro-construction-of-a-banach-limit.md) proves existence even under the stronger convention, rather than leaving shift invariance implicit.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
