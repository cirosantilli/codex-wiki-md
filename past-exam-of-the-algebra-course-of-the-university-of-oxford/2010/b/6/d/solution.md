<h1 id="b/6/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the column order $1,(123),(12)(34),(12345),(13452)$ in $A_5$. The two restrictions of degree four coincide and equal $\theta_4=(4,1,0,-1,-1)$; those of degree five coincide and equal $\theta_5=(5,-1,1,0,0)$. The [centralizer](../../../../../centralizer.md) orders give

$$
\langle\theta_4,\theta_4\rangle=\frac{16}{60}+\frac13+\frac15+\frac15=1,\qquad
\langle\theta_5,\theta_5\rangle=\frac{25}{60}+\frac13+\frac14=1.
$$

Thus both are [irreducible characters](../../../../../irreducible-character.md). The remaining given restriction is $\eta=(6,0,-2,1,1)$, and

$$
\langle\eta,\eta\rangle=\frac{36}{60}+\frac44+\frac15+\frac15=2.
$$

It splits as two distinct [irreducible characters](../../../../../irreducible-character.md). Neither is $1$, $\theta_4$ or $\theta_5$, since their [character inner products](../../../../../character-inner-product.md) with $\eta$ are zero. A finite [group](../../../../../group-split.md) has as many complex [irreducible characters](../../../../../irreducible-character.md) as [conjugacy classes](../../../../../conjugacy-class.md), so these five exhaust them. The sum of squares of irreducible degrees is $|A_5|=60$. The first three degrees contribute $1+16+25=42$, leaving $18$ for the two constituents, whose degrees sum to six. Hence both have degree three.

Write one constituent as $\theta=(3,x,y,u,v)$. All five [conjugacy classes](../../../../../conjugacy-class.md) are closed under inversion, so all its values are real: $\chi(g^{-1})=\overline{\chi(g)}$. Orthogonality with $1$, $\theta_4$ and $\theta_5$ gives

$$
\frac3{60}+\frac x3+\frac y4+\frac{u+v}5=0,\qquad
\frac{12}{60}+\frac x3-\frac{u+v}5=0,\qquad
\frac{15}{60}-\frac x3+\frac y4=0.
$$

Solving gives $x=0$, $y=-1$ and $u+v=1$. The squared [norm](../../../../../norm.md) one gives $9/60+1/4+(u^2+v^2)/5=1$, so $u^2+v^2=3$ and $uv=-1$. Thus $u,v$ are the roots of $t^2-t-1$, namely $\varphi=(1+\sqrt5)/2$ and $\bar\varphi=(1-\sqrt5)/2$. Here the bar labels the other real root, rather than complex conjugation. The other constituent is $\eta-\theta$, so the two last values are interchanged.

The [Character table of the alternating group A5](../../../../../character-table-of-the-alternating-group-a5.md) is therefore

$$
\boxed{\begin{array}{c|rrrrr}
&1&(123)&(12)(34)&(12345)&(13452)\\\hline
1&1&1&1&1&1\\
\theta_3&3&0&-1&\varphi&\bar\varphi\\
\theta'_3&3&0&-1&\bar\varphi&\varphi\\
\theta_4&4&1&0&-1&-1\\
\theta_5&5&-1&1&0&0
\end{array}.}
$$

The [conjugacy class](../../../../../conjugacy-class.md) sizes are $1,20,15,12,12$. A [normal subgroup](../../../../../normal-subgroup.md) is a union of entire [conjugacy classes](../../../../../conjugacy-class.md) containing the identity, and its order divides $60$ by [Lagrange's theorem](../../../../../lagrange-s-theorem.md). A nontrivial such union has size at least $13$; the only proper divisors of $60$ at least $13$ are $15,20,30$. Subtracting the identity would require a sum of some of $20,15,12,12$ equal to $14,19,29$, respectively, none of which is possible. Thus **$A_5$ is simple**.

## ↑ Ancestors (13)

1. [D](../d.md)
2. [6](../../6.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the algebra course of the University of Oxford](../../../../split.md)
6. [Algebra course of the University of Oxford](../../../../../algebra-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
