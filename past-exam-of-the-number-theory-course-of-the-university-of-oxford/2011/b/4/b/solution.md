<h1 id="b/4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [polynomial](../../../../../polynomial-split.md) is irreducible by [Eisenstein's criterion](../../../../../eisenstein-criterion.md) at $q$, so $[K:\mathbb Q]=n$. Its constant coefficient gives the [field norm](../../../../../field-norm.md)

$$
\boxed{N_{K/\mathbb Q}(\theta)=(-1)^na_0.}
$$

The defining equation gives

$$
\frac{r\theta^n}{q}=-r\sum_{j=0}^{n-1}\frac{a_j}{q}\theta^j\in\mathbb Z[\theta]\subseteq\mathcal O_K.
$$

If $q\nmid r$ and $0\le i<n$, then

$$
N_{K/\mathbb Q}\left(\frac{r\theta^i}{q}\right)
=\frac{r^n((-1)^na_0)^i}{q^n}
$$

has $q$-adic valuation $i-n<0$. It is not an [integer](../../../../../integer-split.md). The [norm](../../../../../norm.md) of an [algebraic integer](../../../../../algebraic-integer.md) is an [integer](../../../../../integer-split.md), so $r\theta^i/q$ is not integral.

Suppose now that $\gamma$ is integral. Multiply it by $\theta^{n-1}$. All terms except $r_0\theta^{n-1}/q$ are integral, since their powers of $\theta$ are at least $n$. Thus this remaining term is integral, and the [norm](../../../../../norm.md) obstruction forces $q\mid r_0$. Subtract the [integer](../../../../../integer-split.md) $r_0/q$ from $\gamma$. Multiply the remainder by $\theta^{n-2}$; the only term of exponent below $n$ is $r_1\theta^{n-1}/q$, so $q\mid r_1$. Continuing in this way proves $q\mid r_j$ for every $j$. Therefore

$$
\boxed{\gamma\in\mathbb Z[\theta].}
$$

For $n=1$ the same conclusion follows directly from the [norm](../../../../../norm.md) obstruction with $i=0$.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2011](../../../../2011-split.md)
5. [Past exam of the number theory course of the University of Oxford](../../../../split.md)
6. [Number theory course of the University of Oxford](../../../../../number-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
