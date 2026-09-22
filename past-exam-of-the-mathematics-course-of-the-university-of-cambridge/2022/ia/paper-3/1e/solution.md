<h1 id="1e/solution">Solution</h1>

↑ **Parent:** [1E](../1e.md)

The [order of a group element](../../../../../order-of-a-group-element.md) $g$ is the least [positive integer](../../../../../positive-integer.md) $n$ such that $g^n=e$, where $e$ is the [identity element](../../../../../identity-element.md); its order is infinite if no such $n$ exists.

Let $g$ have finite order $n$. A [group homomorphism](../../../../../group-homomorphism.md) preserves the [group operation](../../../../../group-operation.md) and the identity, so

$$
\phi(g)^n=\phi(g^n)=\phi(e)=e.
$$

The order of an element divides every positive exponent that gives the identity. Hence

$$
\boxed{\operatorname{ord}(\phi(g))\mid\operatorname{ord}(g)}.
$$

If $\phi$ is a [surjective function](../../../../../surjective-function.md) and $h\in H$ has order $m$, choose $g\in G$ with $\phi(g)=h$. The first result gives $m\mid n$, where $n=\operatorname{ord}(g)$. The element

$$
g^{n/m}
$$

then has order $m$, because the order of $g^k$ is $n/\gcd(n,k)$.

A [group homomorphism](../../../../../group-homomorphism.md) $C_9\to S_4$ is determined by the image of a [generator](../../../../../generator-of-a-group.md) of the [cyclic group](../../../../../cyclic-group.md) $C_9$, and that image must have order dividing $9$. In the [symmetric group](../../../../../symmetric-group.md) $S_4$, the only such elements are the identity and the [three-cycles](../../../../../three-cycle.md). There are

$$
\binom43(3-1)!=4\cdot2=8
$$

three-cycles. Therefore the number of homomorphisms is

$$
\boxed{1+8=9}.
$$

## ↑ Ancestors (10)

1. [1E](../1e.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2022](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
