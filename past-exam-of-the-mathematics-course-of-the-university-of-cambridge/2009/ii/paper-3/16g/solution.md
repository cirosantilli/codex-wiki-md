<h1 id="16g/solution">Solution</h1>

↑ **Parent:** [16G](../16g.md)

The induced ordering on $x$ is a [well-order](../../../../../well-order.md). By [transfinite recursion](../../../../../transfinite-recursion.md) define $h(t)=\{h(s):s\in x,\ s<t\}$ for $t\in x$. Induction shows that each $h(t)$ is an [ordinal](../../../../../ordinal.md), that these values strictly increase, and that their range is the [ordinal](../../../../../ordinal.md) $\mu(x)=\bigcup_{t\in x}(h(t)+1)$. The map $h$ is an [order isomorphism](../../../../../order-isomorphism.md) from $x$ to this ordinal. Any [order isomorphism](../../../../../order-isomorphism.md) between ordinals must fix their elements successively, so this ordinal is unique.

An increasing map $j:\kappa\to\lambda$ between [ordinals](../../../../../ordinal.md) satisfies $j(\xi)\ge\xi$ by induction: its predecessors include $j(\eta)$ for all $\eta<\xi$. Hence $\kappa\le\lambda$. Apply this to the inclusion $x\subset y$, transported through their [order isomorphisms](../../../../../order-isomorphism.md), and then to $y\subset\alpha$. It follows that $\boxed{\mu(x)\le\mu(y)\le\alpha}$.

If each $x_n$ is an [initial segment](../../../../../initial-segment.md) of later $x_m$, uniqueness makes their ordinal enumerations compatible: the enumeration of $x_m$ restricts to that of $x_n$. Their union is consequently an [order isomorphism](../../../../../order-isomorphism.md) from $\bigcup_n x_n$ to $\bigcup_n\mu(x_n)$. This proves the asserted equality. Without the [initial segment](../../../../../initial-segment.md) condition it fails: in $\alpha=\omega+1$, take $x_n=\{0,\ldots,n-1\}\cup\{\omega\}$. Then $\mu(x_n)=n+1$, whose union is $\omega$, but $\mu(\bigcup_nx_n)=\omega+1$.

For decreasing sets, $\mu(x_n)$ is a nonincreasing sequence of [ordinals](../../../../../ordinal.md). Its set of values has a least member, attained at some $n_0$; all later values must equal it. Hence the sequence is **eventually constant**. The intersection formula nevertheless fails: take $x_n=\{n,n+1,\ldots\}\subset\omega$. Every $x_n$ has order type $\omega$, whereas their intersection is empty and has order type zero. Thus $\mu(\bigcap_nx_n)=0\ne\bigcap_n\mu(x_n)=\omega$.

## ↑ Ancestors (10)

1. [16G](../16g.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
