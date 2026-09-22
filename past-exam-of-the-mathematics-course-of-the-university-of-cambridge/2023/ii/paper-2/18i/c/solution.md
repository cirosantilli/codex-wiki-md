<h1 id="18i/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $y_1,\ldots,y_r$ be the distinct roots of $g$ in its splitting field $L$. For each $i$, let $x_i$ be the unique $p$th root of $y_i$ in an algebraic closure. Then

$$
T^p-y_i=(T-x_i)^p,
$$

so the roots of

$$
f(T)=g(T^p)
$$

are precisely the $x_i$. Hence

$$
M=L(x_1,\ldots,x_r).
$$

But $y_i=x_i^p$, so $L=K(y_1,\ldots,y_r)\subseteq K(x_1,\ldots,x_r)$. It follows that

$$
M=K(x_1,\ldots,x_r),
$$

which proves that $M$ is also the [splitting field](../../../../../../splitting-field.md) of $f$ over $K$, as in the [splitting field of a polynomial obtained by Frobenius substitution](../../../../../../splitting-field-of-a-polynomial-obtained-by-frobenius-substitution.md).

Moreover $x_i^p=y_i\in L$, so every root of $f$ is purely inseparable over $L$. In fact $M/L$ is purely inseparable.

Now take $\sigma\in\operatorname{Aut}(L/K)$. The [extension theorem for field embeddings](../../../../../../extension-count-for-field-embeddings.md) extends $\sigma$ to a $K$-embedding of $M$ into an algebraic closure. Since $M$ is a splitting field of $f$ over $K$, its image is again $M$, so this extension is an automorphism $\tau$ of $M$. It is unique: for every root $x_i$,

$$
\tau(x_i)^p=\sigma(y_i),
$$

and the [Frobenius endomorphism](../../../../../../frobenius-endomorphism.md) gives only one possible $p$th root. Since the $x_i$ generate $M$ over $L$, $\tau$ is uniquely determined. This is the [unique embedding extension through a purely inseparable extension](../../../../../../unique-embedding-extension-through-a-purely-inseparable-extension.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18I](../../18i.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
