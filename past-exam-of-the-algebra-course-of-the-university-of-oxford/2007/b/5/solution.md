<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

For $|G|=p^rm$ with $p\nmid m$, Sylow's theorem gives subgroups of order $p^r$, says that every $p$-subgroup lies in a conjugate of one of them, and that all such [Sylow subgroups](../../../../sylow-subgroup.md) are conjugate. Their number $n_p$ divides $m$ and satisfies $n_p\equiv1\pmod p$. A [group](../../../../group-split.md) is soluble when its [derived series](../../../../derived-series.md), obtained by repeatedly taking the [commutator subgroup](../../../../commutator-subgroup.md), reaches the identity. Equivalently it has a subnormal series with abelian factors.

For a [group](../../../../group-split.md) of order $p^2$, the [class equation](../../../../class-equation.md) shows its center is nontrivial: noncentral conjugacy classes have sizes divisible by $p$. If the center had order $p$, the quotient by the center would be cyclic; a [group](../../../../group-split.md) with cyclic central quotient is abelian, since representatives are powers of one element times central elements. This would make the center the whole [group](../../../../group-split.md). Thus **every [group](../../../../group-split.md) of order $p^2$ is abelian**.

Now consider $|G|=pq^a$ with $0\leq a\leq2$. Cases with a normal [Sylow subgroup](../../../../sylow-subgroup.md) are soluble: that subgroup has prime or prime-square order and is abelian, and its quotient also has such order and is abelian. This gives a subnormal series with abelian factors.

If $p<q$, the Sylow number $n_q$ divides $p$ and is $1$ modulo $q$, so is one. If $p>q$ and $a\leq1$, $n_p$ divides $q^a<p$, so again is one. For $p>q$ and $a=2$, a nontrivial $n_p$ can only be $q^2$, since $q<p$. The congruence would force $p\mid(q-1)(q+1)$, hence $p\mid q+1$. Since $p>q$, this means $p=q+1$, and primality forces $(p,q)=(3,2)$.

In the remaining order-twelve case, either a [Sylow subgroup](../../../../sylow-subgroup.md) is already normal, or there are four [Sylow subgroups](../../../../sylow-subgroup.md) of order three. Those have pairwise trivial intersection and contribute eight distinct elements of order three. Only four elements remain, including the identity. Every [Sylow subgroup](../../../../sylow-subgroup.md) of order four lies entirely among those four elements, so it is unique and normal. It and its quotient are abelian. Therefore **all [groups](../../../../group-split.md) of the required orders are soluble**, by elementary Sylow arguments alone.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the algebra course of the University of Oxford](../../../split.md)
5. [Algebra course of the University of Oxford](../../../../algebra-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
