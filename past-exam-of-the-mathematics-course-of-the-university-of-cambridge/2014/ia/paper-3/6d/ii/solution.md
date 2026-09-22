<h1 id="6d/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

If a nonidentity power $x^j$ belongs to $H$, reduce $j$ modulo $p$ so that $1\le j<p$. There is an integer $a$ with $aj\equiv1\pmod p$, and therefore $(x^j)^a=x\in H$, a contradiction. Thus

$$
\boxed{\langle x\rangle\cap H=\{1\}.}
$$

Now suppose that $G$ is abelian and finite. Start with $H_0=\{1\}$, and whenever $H_k\ne G$, choose $x_{k+1}\notin H_k$. The multiplication map

$$
H_k\times\langle x_{k+1}\rangle\longrightarrow H_{k+1}=H_k\langle x_{k+1}\rangle
$$

is a [group homomorphism](../../../../../../group-homomorphism.md) because all elements commute. It is surjective by construction and injective because the intersection of its two factors is trivial: $hx=h'x'$ implies $h'^{-1}h=x'x^{-1}$ lies in that intersection. Hence $H_{k+1}\cong H_k\times C_p$, and its order is $p$ times the previous order. Strict growth and finiteness ensure that the construction ends at $G$. Therefore

$$
\boxed{G\cong C_p^n,}
$$

where $n$ is the number of factors, possibly zero. This is an [elementary abelian group](../../../../../../elementary-abelian-group.md), obtained by an explicit [direct product of groups](../../../../../../direct-product-of-groups.md) construction.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [6D](../../6d.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
