<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The set $I^n$ consists precisely of points whose first $n$ positions $x,f(x),\ldots,f^{n-1}(x)$ all lie in $L\cup R$. Hence

$$
\Lambda=\{x\in[0,1]: f^k(x)\in L\cup R\text{ for every }k\geq0\}.
$$

Deleting the first position preserves this condition, proving $f(\Lambda)\subseteq\Lambda$. For the reverse inclusion, if $y\in\Lambda$, take $x=g_L(y)$. Then $x\in L$ and $f^k(x)=f^{k-1}(y)\in L\cup R$ for every $k\geq1$. Thus $x\in\Lambda$ and $f(x)=y$. In fact both [inverse branches](../../../../../inverse-branch.md) give preimages in $\Lambda$. Therefore

$$
\boxed{f(\Lambda)=\Lambda,}
$$

which proves full invariance, not merely forward invariance.

For any infinite symbolic [sequence](../../../../../sequence.md) $s$, the [itinerary cylinders](../../../../../itinerary-cylinder.md) $I_{s_1\cdots s_n}$ are nonempty compact [nested intervals](../../../../../nested-intervals.md). The [nested interval theorem](../../../../../nested-interval-theorem.md) gives at least one point in their intersection. Every $x\in\Lambda$ has a unique itinerary because $L\cap R=\varnothing$. To justify that the itinerary also determines a unique point, it suffices to show the [interval](../../../../../interval-mathematics.md) lengths shrink. The fact that [logistic inverse branches contract in an angular coordinate](../../../../../logistic-inverse-branches-contract-in-an-angular-coordinate.md) works for every $\mu>4$; a direct claim that $|g_L'|,|g_R'|<1$ in the original coordinate would fail for some $\mu$ just above four.

Use the [homeomorphism](../../../../../homeomorphism.md) $h(u)=\sin^2(\pi u/2)$ of $[0,1]$. The transformed [inverse branches](../../../../../inverse-branch.md) are

$$
G_L(u)=h^{-1}(g_L(h(u)))=\frac1\pi\arcsin\left(\frac2{\sqrt\mu}\sin\frac{\pi u}{2}\right),\qquad
G_R(u)=1-G_L(u).
$$

Their [derivatives](../../../../../derivative.md) satisfy

$$
|G_L'(u)|=|G_R'(u)|=
\frac{\cos(\pi u/2)}{\sqrt\mu\sqrt{1-(4/\mu)\sin^2(\pi u/2)}}\leq\frac1{\sqrt\mu}<1.
$$

The inequality follows by squaring and using $4/\mu<1$. Thus every length-$n$ transformed [itinerary cylinder](../../../../../itinerary-cylinder.md) has length at most $\mu^{-n/2}$. Since $|h'|\leq\pi/2$, its original [interval](../../../../../interval-mathematics.md) has length at most $(\pi/2)\mu^{-n/2}$ and shrinks to a point. This gives the claimed one-to-one identification with the one-sided [full shift](../../../../../full-shift.md).

Finally part (ii) gives

$$
f(x)\in\bigcap_{n\geq2} I_{s_2\cdots s_n},\qquad
\boxed{s_1s_2s_3\cdots\ \longmapsto\ s_2s_3\cdots.}
$$

Thus $f$ acts by the [left shift](../../../../../left-shift.md). The identification is a [topological conjugacy](../../../../../topological-conjugacy.md): matching long prefixes forces closeness by the shrinking estimate, while distinct finite [itinerary cylinders](../../../../../itinerary-cylinder.md) are disjoint compact sets and so their inverse coding is [continuous](../../../../../continuous-function.md). In particular $f$ need not be one-to-one on $\Lambda$, just as a one-sided [left shift](../../../../../left-shift.md) has two possible first symbols before any given tail.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the nonlinear systems course of the University of Oxford](../../../../split.md)
6. [Nonlinear systems course of the University of Oxford](../../../../../nonlinear-systems-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
