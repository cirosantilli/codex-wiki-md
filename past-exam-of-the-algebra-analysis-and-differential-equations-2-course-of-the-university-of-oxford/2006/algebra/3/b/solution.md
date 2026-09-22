<h1 id="algebra/3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An element $a$ is a [prime element](../../../../../prime-element.md) when it is nonzero and not a [unit](../../../../../unit-in-a-ring.md), and $a\mid bc$ implies $a\mid b$ or $a\mid c$. If $a=bc$ and $a$ is a [prime element](../../../../../prime-element.md), assume for example $b=ad$. Cancellation in $a=adc$ gives $dc=1$, so $c$ is a [unit](../../../../../unit-in-a-ring.md). This proves every [prime element](../../../../../prime-element.md) is an [irreducible element](../../../../../irreducible-element.md).

In a [Euclidean domain](../../../../../euclidean-domain.md), each nonzero [ideal](../../../../../ideal.md) has a generator of least Euclidean value: division of another member by that generator leaves a remainder in the [ideal](../../../../../ideal.md) of smaller value, so the remainder must vanish. Let $a$ be an [irreducible element](../../../../../irreducible-element.md) and suppose $a\mid bc$ but $a\nmid b$. Write $(a,b)=(d)$. Since $d\mid a$, irreducibility says $d$ is a [unit](../../../../../unit-in-a-ring.md) or is associate to $a$. The second case would give $a\mid b$, so $d$ is a [unit](../../../../../unit-in-a-ring.md). Hence $1=ra+sb$ for some $r,s$. Multiplying by $c$ shows $a\mid c$. Thus **irreducibles in a [Euclidean domain](../../../../../euclidean-domain.md) are prime**.

For $R=\mathbb Z[i\sqrt7]$, use the multiplicative integer [field norm](../../../../../field-norm.md) $N(m+ni\sqrt7)=m^2+7n^2$. [Units](../../../../../unit-in-a-ring.md) have [field norm](../../../../../field-norm.md) one and are exactly $\pm1$. If $2=uv$ were a product of nonunits, their norms would be integers greater than one multiplying to four, hence both would have [field norm](../../../../../field-norm.md) two. But $m^2+7n^2=2$ has no integer solution: $n\ne0$ makes the left side at least seven, and $n=0$ would give $m^2=2$. Therefore **2 is an [irreducible element](../../../../../irreducible-element.md)**.

On the other hand,

$$
(1+i\sqrt7)(1-i\sqrt7)=8
$$

is divisible by 2, while neither factor is, because [divisibility](../../../../../divisibility-split.md) by 2 requires both integer [coefficients](../../../../../coefficient.md) to be even. Thus **2 is not a [prime element](../../../../../prime-element.md)** in this [ring](../../../../../ring.md). It is also **not a [prime element](../../../../../prime-element.md) in $\mathbb Z[i]$**: $2\mid(1+i)^2=2i$, but $2\nmid1+i$. In fact $2=(1+i)(1-i)$ is already a nontrivial [factorization](../../../../../factorization.md) there.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [3](../../3.md)
3. [Algebra](../../../algebra.md)
4. [2006](../../../../2006-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
