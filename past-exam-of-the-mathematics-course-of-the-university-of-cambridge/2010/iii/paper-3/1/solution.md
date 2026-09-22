<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

An [Artinian module](../../../../../artinian-module.md) is an $A$-module satisfying the [descending chain condition](../../../../../descending-chain-condition.md) on [submodules](../../../../../submodule.md): every chain $M_0\supseteq M_1\supseteq\cdots$ is eventually constant. An [Artinian ring](../../../../../artinian-ring.md) is a [ring](../../../../../ring.md) that is [Artinian](../../../../../artinian-ring.md) as a [module](../../../../../module-mathematics.md) over itself, so its descending chains of [ideals](../../../../../ideal.md) stabilize.

We first prove the closure properties needed for finite generation. A [submodule](../../../../../submodule.md) of an [Artinian module](../../../../../artinian-module.md) is [Artinian](../../../../../artinian-ring.md), because any descending chain in it is also a chain in the original [module](../../../../../module-mathematics.md). A [quotient module](../../../../../quotient-module.md) is [Artinian](../../../../../artinian-ring.md), because inverse images turn a descending chain in the quotient into one upstairs. Conversely, consider a [short exact sequence](../../../../../short-exact-sequence.md)

$$
0\longrightarrow N\longrightarrow M\xrightarrow{\pi}Q\longrightarrow0
$$

with $N$ and $Q$ [Artinian](../../../../../artinian-ring.md). For a descending chain $(M_i)$, the chains $M_i\cap N$ and $\pi(M_i)$ both stabilize. Choose $r$ beyond both stabilization indices. If $i\geq r$ and $x\in M_i$, equality of the images gives $y\in M_{i+1}$ with $\pi(y)=\pi(x)$. Then

$$
x-y\in M_i\cap N=M_{i+1}\cap N,
$$

so $x\in M_{i+1}$. Hence $M_i=M_{i+1}$. This proves the extension property of [Artinian modules in a short exact sequence](../../../../../artinian-modules-in-a-short-exact-sequence.md).

Apply this property inductively to $0\to A^{n-1}\to A^n\to A\to0$. Every finite [direct sum](../../../../../direct-sum.md) $A^n$ is [Artinian](../../../../../artinian-ring.md) when $A$ is an [Artinian ring](../../../../../artinian-ring.md). If $m_1,\ldots,m_n$ generate $M$, the map $(a_i)\mapsto\sum a_im_i$ is a [surjection](../../../../../surjective-function.md) $A^n\twoheadrightarrow M$. The quotient property therefore proves

$$
\boxed{A\text{ Artinian and }M\text{ finitely generated}\ \Longrightarrow\ M\text{ Artinian}.}
$$

This argument also covers the zero [module](../../../../../module-mathematics.md); it does not require a structure theorem for [Artinian rings](../../../../../artinian-ring.md).

For a counterexample without finite generation, take any [field](../../../../../field.md) $k$ and the [module](../../../../../module-mathematics.md)

$$
M=\bigoplus_{j\geq0}ke_j,\qquad M_i=\bigoplus_{j\geq i}ke_j.
$$

The [ring](../../../../../ring.md) $k$ is [Artinian](../../../../../artinian-ring.md), since its only [ideals](../../../../../ideal.md) are $0$ and $k$. But $M_i\supsetneq M_{i+1}$ for every $i$, since $e_i\notin M_{i+1}$. Thus **an infinite-dimensional [vector space](../../../../../vector-space-split.md) over a [field](../../../../../field.md) provides the requested non-Artinian [module](../../../../../module-mathematics.md)**.

Finally, let $f:M\to M$ be an injective [endomorphism](../../../../../endomorphism.md) with $M$ [Artinian](../../../../../artinian-ring.md). Its image chain stabilizes, so $f^rM=f^{r+1}M$ for some $r$. Given $x\in M$, choose $y$ with $f^rx=f^{r+1}y=f^r(fy)$. Since $f^r$ is injective, $x=fy$. Therefore

$$
\boxed{f\text{ injective}\ \Longrightarrow\ f\text{ surjective}.}
$$

This is precisely the assertion that [Artinian modules are co-Hopfian](../../../../../artinian-modules-are-co-hopfian.md).

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 3](../../paper-3-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
