<h1 id="b/4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

An [integral basis](../../../../integral-basis.md) is a $\mathbb Z$-[basis](../../../../basis.md) of the [ring of integers](../../../../ring-of-integers.md) $\mathcal O_K$; its elements also form a $\mathbb Q$-[basis](../../../../basis.md) of $K$.

To prove existence, first multiply the elements of a rational [basis](../../../../basis.md) by suitable nonzero integers to obtain an integral rational [basis](../../../../basis.md) $w_1,\ldots,w_n$. Put $M=\sum_j\mathbb Zw_j$. The trace pairing is nondegenerate in characteristic zero, and the matrix $T=(\operatorname{Tr}(w_iw_j))$ has [integer](../../../../integer-split.md) entries and nonzero determinant $\Delta$. If $\alpha=\sum_jc_jw_j$ is integral, all $\operatorname{Tr}(\alpha w_i)$ are integers, so $Tc\in\mathbb Z^n$. The adjugate formula gives $c\in\Delta^{-1}\mathbb Z^n$. Consequently

$$
M\subseteq\mathcal O_K\subseteq\Delta^{-1}M.
$$

A [subgroup](../../../../subgroup.md) of a free [abelian group](../../../../abelian-group.md) is free, and these inclusions force rank $n$. A $\mathbb Z$-[basis](../../../../basis.md) of $\mathcal O_K$ is therefore an [integral basis](../../../../integral-basis.md).

Now put $s=\theta^2=\sqrt d$ and $F=\mathbb Q(s)$. The [polynomial](../../../../polynomial-split.md) $X^4-d$ is irreducible by Eisenstein at any prime dividing the squarefree $d$, except for $d=-1$, where $(X+1)^4+1$ is Eisenstein at $2$. Thus $[K:\mathbb Q]=4$ and $[K:F]=2$. Every $\gamma\in K$ has the unique form $\alpha+\beta\theta$ with $\alpha,\beta\in F$. The nontrivial $F$-[automorphism](../../../../automorphism.md) sends $\theta$ to $-\theta$, so an integral $\gamma$ has integral conjugate $\alpha-\beta\theta$. Relative trace and [norm](../../../../norm.md) of integral elements are integral in $F$. Applying them to $\gamma$ and taking the trace of $\theta\gamma$ gives

$$
\boxed{2\alpha,\quad\alpha^2-\beta^2s,\quad2\beta s\in\mathcal O_F=\mathbb Z[s].}
$$

The [power basis](../../../../power-basis.md) has [discriminant](../../../../discriminant.md)

$$
\boxed{\operatorname{disc}(1,\theta,\theta^2,\theta^3)=-256d^3.}
$$

Indeed, the resultant of $X^4-d$ and $4X^3$ is $4^4\prod\theta_j^3=-256d^3$; the [discriminant](../../../../discriminant.md) sign factor is $(-1)^6=1$. By the [discriminant-index formula for an integral lattice](../../../../discriminant-index-formula-for-an-integral-lattice.md), a prime dividing $[\mathcal O_K:\mathbb Z[\theta]]$ must divide $2d$.

No odd prime $p\mid d$ can divide this index. The Eisenstein equation gives $\theta^4/p\in\mathcal O_K$, while $r\theta^i/p$ has nonintegral [field norm](../../../../field-norm.md) for $p\nmid r$ and $0\le i<4$: its $p$-adic [norm](../../../../norm.md) valuation is $i-4<0$. If $p^{-1}\sum_{i=0}^3r_i\theta^i$ were integral, multiplication by $\theta^3$ first forces $p\mid r_0$; subtracting $r_0/p$ and multiplying by $\theta^2$ forces $p\mid r_1$. Continuing forces all coefficients divisible by $p$. This excludes an index element of order $p$.

To exclude $2$, any index element of order two would be represented by an integral

$$
\gamma=\frac{a+b\theta+c\theta^2+e\theta^3}{2}
$$

with integers $a,b,c,e$ not all even. Here $\alpha=(a+cs)/2$ and $\beta=(b+es)/2$. The integrality of $\alpha^2-\beta^2s$ forces

$$
a^2+dc^2-2dbe\equiv0\pmod4,\qquad
2ac-b^2-de^2\equiv0\pmod4.
$$

Since $d\equiv3\pmod4$, the first congruence implies $a,c$ have the same parity. If both were odd, the second would require $b^2+3e^2\equiv2\pmod4$, impossible. Hence $a,c$ are even. The second congruence then forces $b,e$ to have the same parity, while the first forces $be$ even. Thus $b,e$ are even too, a contradiction. Therefore the index is one and

$$
\boxed{\mathcal O_K=\mathbb Z[\theta],\qquad(1,\theta,\theta^2,\theta^3)\text{ is an integral basis}.}
$$

For the last request, let $t=\sqrt[4]5$ and take $\delta=(t+t^3)/2$. It satisfies $\delta^2=(5+3\sqrt5)/2$, and hence

$$
\boxed{\delta^4-5\delta^2-5=0.}
$$

This monic [integer](../../../../integer-split.md) [polynomial](../../../../polynomial-split.md) proves integrality. Its coordinates in the rational power [basis](../../../../basis.md) have halves, so $\delta\notin\mathbb Z[t]$. Also $\delta=t(1+\sqrt5)/2$ with a nonzero coefficient in $\mathbb Q(\sqrt5)$; if $\delta$ were in that [quadratic field](../../../../quadratic-field.md), then $t$ would be too, contradicting degree four. Thus it meets both exclusions.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [B](../../b.md)
3. [2010](../../../2010-split.md)
4. [Past exam of the number theory course of the University of Oxford](../../../split.md)
5. [Number theory course of the University of Oxford](../../../../number-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
