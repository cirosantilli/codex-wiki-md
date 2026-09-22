<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The [integral closure](../../../../../integral-closure.md) of $R$ in $T$ is

$$
\overline R^{\,T}=\{t\in T:t\text{ satisfies a monic polynomial over }R\}.
$$

It is a subring: finitely many integral elements generate a finite $R$-module algebra, and the [determinant trick](../../../../../determinant-trick.md) shows that each element of that algebra is integral. In particular, sums and products of integral elements remain integral.

A [valuation ring](../../../../../valuation-ring.md) is an [integral domain](../../../../../integral-domain.md) $V$ such that, for every nonzero $z$ in its [fraction field](../../../../../field-of-fractions.md), either $z\in V$ or $z^{-1}\in V$. Equivalently, its [ideals](../../../../../ideal.md) are totally ordered by inclusion. For principal [ideals](../../../../../ideal.md), comparability is precisely the condition on $a/b$; if two arbitrary [ideals](../../../../../ideal.md) were incomparable, elements chosen from their differences would contradict principal-ideal comparability. Such a [ring](../../../../../ring.md) is local. Its nonunits form an [ideal](../../../../../ideal.md): if $a,b$ are nonunits and, for example, $b/a\in V$, then $a+b=a(1+b/a)$ is still a nonunit. The unique [maximal ideal](../../../../../maximal-ideal.md) consists of those nonunits.

First, [valuation rings are integrally closed](../../../../../valuation-rings-are-integrally-closed.md). If $z\notin V$, then $y=z^{-1}\in V$ is a nonunit and lies in its [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak m$. A monic relation for $z$ over $V$, multiplied by $y^n$, would give

$$
1+a_{n-1}y+\cdots+a_0y^n=0,
$$

which is impossible modulo $\mathfrak m$. Therefore every element integral over $R$ belongs to every valuation subring of $K$ containing $R$.

For the reverse inclusion, we will construct a valuation overring that excludes any chosen nonintegral element. We need the [valuation domination lemma](../../../../../valuation-domination-lemma.md): a local subring $(A,\mathfrak n)$ of a [field](../../../../../field.md) $K$ is dominated by a valuation subring $V$ of $K$, meaning $A\subseteq V$ and $\mathfrak m_V\cap A=\mathfrak n$. Here is a proof, including the crucial maximality step.

Order the local subrings of $K$ dominating $A$ by domination. For a chain, take the union of the [rings](../../../../../ring.md) and of their maximal [ideals](../../../../../ideal.md). The union is a [local ring](../../../../../local-ring.md): an element outside the union [ideal](../../../../../ideal.md) is already a unit in a member of the chain, while an element in that [ideal](../../../../../ideal.md) cannot become a unit in a later dominating member. The union still dominates $A$. Thus [Zorn's lemma](../../../../../zorn-s-lemma.md) supplies a maximal pair $(V,\mathfrak m)$.

For any $z\in K^\times$, at least one of $\mathfrak mV[z]$ and $\mathfrak mV[z^{-1}]$ is proper. Suppose otherwise. There would be relations

$$
1=\sum_{i=0}^n a_i z^i,\qquad1=\sum_{j=0}^s b_j z^{-j},\qquad a_i,b_j\in\mathfrak m,
$$

with $n,s$ chosen minimal. Both are positive. Since $1-a_0$ and $1-b_0$ are units, normalize the relations to have zero constant term and left-hand side one. If $n\geq s$, the second relation gives

$$
z^s=\sum_{j=1}^s c_jz^{s-j},\qquad c_j\in\mathfrak m.
$$

Repeatedly substituting this monic reduction in the first relation yields a relation for $1$ of degree less than $s$, with every coefficient still in $\mathfrak m$. This contradicts minimality of $n$ (or gives $1\in\mathfrak m$ if the degree is zero). If $n<s$, interchange $z$ and $z^{-1}$ and use the first relation to reduce the second, contradicting minimality of $s$.

Choose whichever extension has a proper extended [ideal](../../../../../ideal.md), then a [maximal ideal](../../../../../maximal-ideal.md) containing it. Localizing that extension at the chosen [maximal ideal](../../../../../maximal-ideal.md) produces a [local ring](../../../../../local-ring.md) dominating $V$. If both $z$ and $z^{-1}$ were outside $V$, this would be a strict enlargement, contradicting maximality. Thus $V$ has the valuation property. In particular its [fraction field](../../../../../field-of-fractions.md) is all of $K$, since each nonzero element of $K$ or its inverse belongs to $V$. This proves the [valuation domination lemma](../../../../../valuation-domination-lemma.md).

Now let $x\in K$ be nonintegral over $R$, so $x\neq0$, and set $y=x^{-1}$, $B=R[y]$. The [ideal](../../../../../ideal.md) $yB$ is proper: otherwise $1=y(r_0+r_1y+\cdots+r_ny^n)$, and multiplication by $x^{n+1}$ gives a monic equation for $x$ over $R$. Choose a [maximal ideal](../../../../../maximal-ideal.md) $\mathfrak n$ of $B$ containing $y$, and apply the [valuation domination lemma](../../../../../valuation-domination-lemma.md) to $B_{\mathfrak n}\subset K$. Its dominating [valuation ring](../../../../../valuation-ring.md) $V$ contains $R$ and has $y\in\mathfrak m_V$. Hence $y$ is not invertible in $V$, so $x\notin V$.

We have excluded every nonintegral element from at least one valuation overring, while every integral element belongs to all of them. Therefore the [integral closure as an intersection of valuation rings](../../../../../integral-closure-as-an-intersection-of-valuation-rings.md) is

$$
\boxed{\overline R^{\,K}=\bigcap_{\substack{V\subseteq K\text{ a valuation ring}\\R\subseteq V}}V.}
$$

Neither [Noetherianity](../../../../../noetherian-ring.md) nor a discrete valuation is required for this separation argument.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
