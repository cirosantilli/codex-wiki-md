<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

It is enough to consider three alternatives $A,B,C$. Encode each voter's three pairwise preferences by $(x_i,y_i,z_i)$, where $x_i=1$ means $A>B$, $y_i=1$ means $B>C$, and $z_i=1$ means $C>A$. A valid ranking excludes $(1,1,1)$ and $(-1,-1,-1)$. Independence of irrelevant alternatives gives three [Boolean functions](../../../../../../boolean-function.md) $u,v,w$ for the social comparisons. Unanimity and transitivity force $u=v=w$: fixing arbitrary $x$, taking $y=-x$ and $z$ constantly equal to $u(x)$ shows $v(-x)=-u(x)$, and cyclic symmetry gives the claim.

Choose the voters' valid rankings independently and uniformly. A social [Condorcet paradox](../../../../../../condorcet-paradox.md) is absent exactly when

$$
u(x)u(y)+u(y)u(z)+u(z)u(x)=-1.
$$

Thus transitivity for every profile gives $3\mathbb E[u(x)u(y)]=-1$. Conditional on $x_i$, the bit $y_i$ equals $x_i$ with probability $1/3$ and differs with probability $2/3$, so $(x,y)$ has correlation $-1/3$. Therefore

$$
\operatorname{Stab}_{-1/3}(u)=-\frac13.
$$

The Fourier formula, valid for negative correlation, gives

$$
\sum_{S\subseteq[n]}\left(-\frac13\right)^{|S|}\widehat u(S)^2=-\frac13,
\qquad
\sum_S\widehat u(S)^2=1
$$

by [Parseval identity](../../../../../../parseval-identity.md). Among the numbers $(-1/3)^m$, the unique minimum is $-1/3$, attained at $m=1$. Equality in this weighted average therefore forces all Fourier mass onto level one. Hence $u$ is a linear Boolean function with zero constant term. Such a function can have only one nonzero coefficient: otherwise varying two coordinates would make it assume more than two values. Thus $u(x)=x_j$ or $u(x)=-x_j$ for some $j$, making voter $j$ a dictator and proving [Arrow theorem](../../../../../../arrow-s-impossibility-theorem.md).

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 168](../../../paper-168-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
