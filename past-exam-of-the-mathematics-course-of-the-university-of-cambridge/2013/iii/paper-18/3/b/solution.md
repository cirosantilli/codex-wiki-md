<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Construct [pointwise limits in a functor category](../../../../../../pointwise-limits-in-a-functor-category.md). For $H:\mathcal J\to[\mathcal D,\mathcal C]$, choose at each object $d$ a [categorical limit](../../../../../../categorical-limit.md) $L(d)$ of $j\mapsto H_j(d)$, with projections $p_j(d)$. For $u:d\to d'$, the family $H_j(u)p_j(d)$ is compatible; define $L(u)$ uniquely by

$$
p_j(d')L(u)=H_j(u)p_j(d).
$$

The [universal property](../../../../../../universal-property.md) gives $L(1_d)=1_{L(d)}$ and $L(vu)=L(v)L(u)$, since those equalities hold after every projection. Thus $L$ is a [functor](../../../../../../functor.md), and each $p_j:L\Rightarrow H_j$ is a [natural transformation](../../../../../../natural-transformation.md).

For any [categorical cone](../../../../../../cone-over-a-diagram.md) $(M,(a_j))$, the pointwise [categorical limits](../../../../../../categorical-limit.md) give unique maps $a(d):M(d)\to L(d)$. To check naturality, compose $L(u)a(d)$ and $a(d')M(u)$ with every $p_j(d')$; both become $H_j(u)a_j(d)=a_j(d')M(u)$. The projections distinguish arrows into their [categorical limit](../../../../../../categorical-limit.md), so the two maps agree. Componentwise uniqueness gives uniqueness of the [natural transformation](../../../../../../natural-transformation.md) $a$. This proves that $(L,p_j)$ really is the required [categorical limit](../../../../../../categorical-limit.md), rather than merely a family of objectwise candidates.

A specified [categorical limit](../../../../../../categorical-limit.md) [categorical cone](../../../../../../cone-over-a-diagram.md) in $\mathcal C^{\operatorname{ob}\mathcal D}$ fixes these objectwise vertices and projections. The displayed equation forces every arrow $L(u)$, and the argument forces every [categorical cone](../../../../../../cone-over-a-diagram.md) factorization. Hence the [forgetful functor](../../../../../../forgetful-functor.md) uniquely lifts that [categorical cone](../../../../../../cone-over-a-diagram.md) and is a [limit-creating functor](../../../../../../limit-creating-functor.md). The construction only takes small [categorical limits](../../../../../../categorical-limit.md) in $\mathcal C$; it does not require $\mathcal D$ to be small. As usual, the [functor categories](../../../../../../functor-category.md) are understood in a universe where their collections of transformations are meaningful.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 18](../../../paper-18-split.md)
4. [Iii](../../../split.md)
5. [2013](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
