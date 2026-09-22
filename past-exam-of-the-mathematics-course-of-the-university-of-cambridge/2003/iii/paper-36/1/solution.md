<h1 id="1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

For a [linear code](../../../../../linear-code.md) $X\leq\mathbb F^n$, its [dual code](../../../../../dual-code.md) is

$$
X^\perp=\{y\in\mathbb F^n:\sum_{i=1}^n x_i y_i=0\text{ for every }x\in X\}.
$$

The standard [bilinear form](../../../../../bilinear-form.md) is nondegenerate. The map $\mathbb F^n\to X^*$ obtained by restricting the dot-product functional to $X$ is [surjective](../../../../../surjective-function.md): extend a functional from a [basis](../../../../../basis.md) of $X$ to a [basis](../../../../../basis.md) of $\mathbb F^n$, then use the nondegenerate [dot product](../../../../../dot-product.md) to represent it. Its [kernel](../../../../../kernel-of-a-linear-map.md) is $X^\perp$. The [rank-nullity theorem](../../../../../rank-nullity-theorem.md) therefore gives

$$
\boxed{\dim X^\perp=n-\dim X.}
$$

The first proposed description of the [dual code](../../../../../dual-code.md) is **false without self-orthogonality**. At length three take $X=\langle(1,0,0)\rangle$. It has the specified [dimension](../../../../../dimension-vector-space.md), but

$$
X^\perp=\{(0,a,b):a,b\in\mathbb F_2\},
$$

whereas $\langle X,(1,1,1)\rangle$ contains $(1,0,0)$ and $(1,1,1)$, neither of which is in $X^\perp$. The natural corrected statement is the [odd-length binary self-orthogonal dual extension](../../../../../odd-length-binary-self-orthogonal-dual-extension.md): if also $X\subseteq X^\perp$, every word of $X$ has even [Hamming weight](../../../../../hamming-weight.md), the all-ones word lies in $X^\perp$ but not in $X$, and [dimensions](../../../../../dimension-vector-space.md) then give $X^\perp=X\oplus\langle\mathbf1\rangle$.

For a binary [self-dual code](../../../../../self-dual-code.md), $x\cdot x=0$ for every $x\in X$. In $\mathbb F_2$, this equals $\sum_i x_i$, so every [codeword](../../../../../codeword.md) has even [Hamming weight](../../../../../hamming-weight.md). Thus $\mathbf1\cdot x=0$ for all $x$, giving $\mathbf1\in X^\perp=X$. The [dimension](../../../../../dimension-vector-space.md) identity yields $2\dim X=n$, so $n$ is even. Alternatively $\mathbf1\in X$ and $\mathbf1\cdot\mathbf1=0$ itself gives evenness. Hence **the second assertion is true**.

For every $n=2m$, use

$$
X=\{(u,u):u\in\mathbb F_2^m\},\qquad G=(I_m\mid I_m).
$$

This [linear code](../../../../../linear-code.md) has [dimension](../../../../../dimension-vector-space.md) $m$, and $(u,u)\cdot(v,v)=2(u\cdot v)=0$. Therefore $X\subseteq X^\perp$; both have [dimension](../../../../../dimension-vector-space.md) $m$, so equality holds. This constructs a binary [self-dual code](../../../../../self-dual-code.md) at every even length. Conversely the [dimension](../../../../../dimension-vector-space.md) identity already proves **every self-dual length-$n$ [linear code](../../../../../linear-code.md) has [dimension](../../../../../dimension-vector-space.md) $n/2$**.

For a nonbinary example, over $\mathbb F_5$ take $X=\langle(1,2)\rangle$. Its generator has self-product $1+2^2=0$ in $\mathbb F_5$, so $X\subseteq X^\perp$. Both are one-dimensional, proving

$$
\boxed{\langle(1,2)\rangle\leq\mathbb F_5^2\text{ is self-dual}.}
$$

## ↑ Ancestors (10)

1. [1](../1.md)
2. [Paper 36](../../paper-36-split.md)
3. [Iii](../../split.md)
4. [2003](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
