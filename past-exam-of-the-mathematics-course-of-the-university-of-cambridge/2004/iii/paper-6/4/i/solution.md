<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $p$ be the [Minkowski functional](../../../../../../minkowski-functional.md) of $E$:

$$
p(v)=\inf\{t>0:v\in tE\}.
$$

The contained ball makes $E$ absorbing, so $p$ is finite, nonnegative and satisfies $p(v)\leq\|v\|/\epsilon$. It is positively homogeneous. To check subadditivity, if $v\in sE$ and $w\in tE$, the defining property of a [convex set](../../../../../../convex-set.md) gives $(v+w)/(s+t)\in E$, whence $p(v+w)\leq s+t$; let $s,t$ decrease to the respective infima. Thus $p$ is a [sublinear functional](../../../../../../sublinear-function.md). We have $p(e)\leq1$ for every $e\in E$. Also $p(x)\geq1$: otherwise $x\in tE$ for some $0<t<1$, which would put $x$ in $E$ because $E$ is a [convex set](../../../../../../convex-set.md) and $0\in E$.

We prove the dominated form of the [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md) needed here. Suppose $g$ is linear on a subspace $M$ and $g\leq p$ there. To extend it to $M+\mathbb Rv$ with $v\notin M$, choose the value $c$ at $v$ between

$$
\sup_{m\in M}\{g(m)-p(m-v)\}
\quad\text{and}\quad
\inf_{n\in M}\{p(n+v)-g(n)\}.
$$

Every lower candidate is at most every upper candidate, because

$$
g(m)+g(n)=g(m+n)\leq p(m+n)\leq p(m-v)+p(n+v).
$$

Taking $m=n=0$ among the candidates shows the two endpoints are finite: the lower supremum is at least $-p(-v)$ and at most $p(v)$, and the upper infimum lies between them and $p(v)$. Define $\widetilde g(m+tv)=g(m)+tc$. For $t>0$, the upper inequality applied to $m/t$ gives domination by $p(m+tv)$. For $t<0$, apply the lower inequality to $m/(-t)$ and multiply by $-t$. At $t=0$ domination already holds. Hence this is a dominated one-dimensional extension.

Order all dominated extensions by inclusion of their domains. Chain unions preserve linearity and domination, so [Zorn's lemma](../../../../../../zorn-s-lemma.md) gives a maximal extension. The one-dimensional argument shows its domain is the whole vector space. This proves the requisite dominated [Hahn-Banach theorem](../../../../../../hahn-banach-theorem.md), rather than invoking an unproved separation form.

On the line $\mathbb Rx$, start with $g(tx)=tp(x)$. For $t\geq0$ this equals $p(tx)$; for $t<0$ it is nonpositive and therefore at most $p(tx)$. Extend it to $T\leq p$ on $V$. Then

$$
Tx=p(x)\geq1,\qquad Te\leq p(e)\leq1\quad(e\in E).
$$

Applying domination to $v$ and $-v$ also gives

$$
|Tv|\leq\frac{\|v\|}{\epsilon}.
$$

Thus $T$ is a [continuous linear functional](../../../../../../continuous-linear-functional.md), and

$$
\boxed{Tx\geq1\geq Te\quad\text{for every }e\in E.}
$$

This proves [separation from an absorbing convex set](../../../../../../separation-from-an-absorbing-convex-set.md) with no closedness assumption on $E$. The proof also gives the norm-preserving real extension theorem used earlier: take $p(v)=C\|v\|$ when the original functional has [norm](../../../../../../norm.md) at most $C$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 6](../../../paper-6-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
