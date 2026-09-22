<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Consider the subalgebra

$$
\boxed{A=\mathbb C+x\mathbb C[x,y]=\mathbb C[x,xy,xy^2,xy^3,\ldots]\subseteq\mathbb C[x,y].}
$$

It is closed under multiplication because every nonconstant term of its elements is divisible by $x$. Evaluation at $x=0$ defines a homomorphism $A\to\mathbb C$ with kernel $I=x\mathbb C[x,y]$. Its square is $I^2=x^2\mathbb C[x,y]$, so

$$
I/I^2\cong x\mathbb C[y]
$$

as a complex [vector space](../../../../../../vector-space-split.md). In particular, the classes of $xy^j$, $j\ge0$, are linearly independent and span it.

If $A$ were a [finitely generated algebra](../../../../../../finitely-generated-algebra.md), take a finite list of generators and subtract their scalar images under evaluation. The resulting generators $z_1,\ldots,z_r$ lie in $I$ and still generate $A$ over $\mathbb C$. Every element of $I$ is a polynomial in the $z_i$ with zero constant term. Modulo $I^2$, all terms of degree at least two vanish, leaving a linear combination of the classes of $z_1,\ldots,z_r$. This would make $I/I^2$ finite-dimensional, contradicting the displayed infinite basis. Thus **this subalgebra is not finitely generated**. This is the [infinite cotangent space obstructs finite algebra generation](../../../../../../infinite-cotangent-space-obstructs-finite-algebra-generation.md) argument; it proves failure of finite generation even when the proposed generators are arbitrary polynomials, rather than just monomials.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 15](../../../paper-15-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
