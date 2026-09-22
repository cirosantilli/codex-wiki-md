<h1 id="10e/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Evaluation at a real point defines a surjective [ring homomorphism](../../../../../../ring-homomorphism.md) $p\mapsto p(a,b)$ from $\mathbb R[x,y]$ to $\mathbb R$. Its [kernel](../../../../../../kernel-of-a-linear-map.md) is $(x-a,y-b)$: subtracting the constant $p(a,b)$ expresses the remainder as a multiple of $x-a$ plus a multiple of $y-b$, by successive [polynomial division](../../../../../../polynomial-division.md). The [first isomorphism theorem](../../../../../../first-isomorphism-theorem.md) therefore identifies the [quotient ring](../../../../../../quotient-ring.md) with the [field](../../../../../../field.md) $\mathbb R$, proving **each $I_{a,b}$ is maximal**.

For a [maximal ideal](../../../../../../maximal-ideal.md) not on this list, take

$$
\boxed{J=(x^2+1,y).}
$$

Evaluation $p(x,y)\mapsto p(i,0)$ is onto $\mathbb C$, and its [kernel](../../../../../../kernel-of-a-linear-map.md) is $J$: first subtract a multiple of $y$, then divide the remaining polynomial in $x$ by $x^2+1$. Hence $\mathbb R[x,y]/J\cong\mathbb C$, a [field](../../../../../../field.md). Finally, if $J=I_{a,b}$ for real $a,b$, the member $x^2+1\in J$ would vanish at $(a,b)$, requiring $a^2+1=0$, which is impossible over $\mathbb R$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [10E](../../10e.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
