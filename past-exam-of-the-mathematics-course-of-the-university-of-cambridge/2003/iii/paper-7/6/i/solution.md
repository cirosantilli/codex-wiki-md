<h1 id="6/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

We use the [Bose-Chowla Sidon construction](../../../../../../bose-chowla-sidon-construction.md), deriving its difference property explicitly. Let $p$ be an odd prime and choose a generator $\theta$ of the [multiplicative group of a finite field](../../../../../../multiplicative-group-of-a-finite-field.md) of the quadratic [finite field extension](../../../../../../finite-field-extension.md) $\mathbb F_{p^2}$. Such a generator cannot belong to $\mathbb F_p$, so $1,\theta$ are linearly independent over the prime field. For each $t\in\mathbb F_p$, the nonzero field element $\theta+t$ has a unique exponent $a_t$ modulo $p^2-1$, with $\theta^{a_t}=\theta+t$. The $p$ exponents are distinct.

Suppose $a_s-a_t=a_u-a_v$ in the [cyclic group](../../../../../../cyclic-group.md). Multiplying the corresponding field elements gives

$$
(\theta+s)(\theta+v)=(\theta+u)(\theta+t).
$$

Subtract the common $\theta^2$ term. Linear independence of $1,\theta$ gives $s+v=u+t$ and $sv=ut$. Thus the two unordered pairs are the roots of the same monic [quadratic polynomial](../../../../../../quadratic-polynomial.md), so $\{s,v\}=\{u,t\}$. Either $s=u,v=t$, giving the same ordered difference, or $s=t,v=u$, giving two zero differences. This is exactly the [Sidon set](../../../../../../sidon-set.md) property.

Choose the integer representatives in $\{1,\ldots,p^2-1\}$. Equality of integer differences implies equality modulo $p^2-1$, so their Sidon property persists in the integers. Now apply the given prime-gap hypothesis at $x=\sqrt N$ to get $\sqrt N-N^{3/8}\leq p\leq\sqrt N$ for large $N$. The representatives fit inside $\{1,\ldots,N\}$, because $p^2-1\leq N$, and their [cardinality](../../../../../../cardinality.md) is

$$
\boxed{|A|=p\geq\sqrt N-N^{3/8}=\sqrt N-o(\sqrt N).}
$$

Only the supplied short-interval prime existence and the elementary structure of a finite field are used.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [6](../../6.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
