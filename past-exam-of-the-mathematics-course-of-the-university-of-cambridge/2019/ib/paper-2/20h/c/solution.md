<h1 id="20h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $v_i$ be the vertex $i$ steps from $B$ toward $C$, and let $x_i$ be the mean time to reach $v_{i+1}$ from $v_i$. Part (b) gives $x_0=4n+1$. For $1\leq i<n$, first-step analysis at $v_i$ gives

$$
x_i=\frac12\cdot1+\frac12(1+x_{i-1}+x_i),
$$

because a step to $v_{i-1}$ must be followed by a fresh passage of mean $x_{i-1}$ back to $v_i$ before trying again. Hence

$$
x_i=x_{i-1}+2=4n+1+2i.
$$

By the [Strong Markov property](../../../../../../strong-markov-property.md), the expected time from $B$ to $C$ is the sum of these successive passage times:

$$
\mathbb E_B[T_C]
=\sum_{i=0}^{n-1}x_i
=n(4n+1)+n(n-1)=5n^2.
$$

Adding the initial mean time $n^2$ from $A$ to $B$ gives

$$
\boxed{\mathbb E_A[T_C]=6n^2}.
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [20H](../../20h.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
