<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For this [equal-strength power-law mutual repression](../../../../../../equal-strength-power-law-mutual-repression.md), the logarithmic gains and their product at equilibrium are

$$
\epsilon_f=-\frac{ny}{1+y},\qquad \epsilon_g=-\frac{mx}{1+x},\qquad
P=\epsilon_f\epsilon_g=\frac{mnxy}{(1+x)(1+y)}.
$$

The [mutual repression stability criterion](../../../../../../mutual-repression-stability-criterion.md) immediately excludes [multistability](../../../../../../multistability.md) if $mn\le1$, since $P<mn$ at every finite positive equilibrium. The common prefactor $\lambda$ gives a stronger exclusion: **if either exponent is at most one, multistability is impossible for every $\lambda$**, including some cases with $mn>1$.

To prove the additional cases, suppose $m\le1<n$. At equilibrium the two expressions for $\lambda$ imply

$$
\frac{x}{(1+x)^m}=\frac{y}{(1+y)^n}.
$$

Put $a=x/(1+x)$ and $b=y/(1+y)$. Because $m\le1$, the left side is at least $a$, so $a\le b(1-b)^{n-1}$. It follows that

$$
P=mnab\le mn b^2(1-b)^{n-1}
\le\frac{4mn(n-1)^{n-1}}{(n+1)^{n+1}}<1.
$$

The maximum in the second inequality occurs at $b=2/(n+1)$. Its strict bound follows from $4n/(n+1)^2\le1$, $m\le1$, and $((n-1)/(n+1))^{n-1}<1$. Interchanging the components proves the case $n\le1<m$; the case with both exponents at most one was already covered by $mn\le1$. Every root of $F(x)=f(g(x))-x$ therefore has $F'<0$. Since $F$ begins positive and ends negative, there is exactly one root: two downward crossings would require another crossing with nonnegative derivative between them. The unique equilibrium is stable.

For completeness, neither exponent can be relaxed above one in this exclusion. If $m>1$ and $n>1$, take $\lambda$ sufficiently large. On $x\in[\lambda/2,\lambda]$, $g(x)=O(\lambda^{1-m})\to0$, so $f(g(x))=\lambda(1+o(1))$ maps that interval into itself. It has a fixed point with

$$
x\sim\lambda,\qquad y\sim\lambda^{1-m},\qquad P\to0.
$$

It is a [stable equilibrium](../../../../../../stable-equilibrium.md). By exchanging the components, there is a second stable fixed point with $y\sim\lambda$ and $x\sim\lambda^{1-n}$. These two regions are disjoint for large $\lambda$, proving [bistability](../../../../../../bistability.md) for some production strength. Hence the full answer is

$$
\boxed{\text{No multistability for any }\lambda>0\quad\Longleftrightarrow\quad m\le1\ \text{or}\ n\le1.}
$$

For example, $m=1/2,n=3$ has $mn>1$ but still a unique stable equilibrium for all $\lambda$. Thus the product-only necessary condition for strong feedback is not sufficient when both production prefactors are constrained to be equal.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 74](../../../paper-74-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
