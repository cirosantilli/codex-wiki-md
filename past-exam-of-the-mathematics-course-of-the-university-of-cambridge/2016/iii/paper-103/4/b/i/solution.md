<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For $k=1$, the product is empty and equals the identity, the only $1$-cycle in $S_1$. Suppose the [cycle-sum identity for Young–Jucys–Murphy elements](../../../../../../../cycle-sum-identity-for-young-jucys-murphy-elements.md) holds at $k-1$:

$$
X_2\cdots X_{k-1}=\sum_{\sigma\text{ a }(k-1)\text{-cycle}}\sigma.
$$

Multiplication by $X_k=\sum_{a<k}(a\ k)$ gives terms $\sigma(a\ k)$. With permutation products acting right to left, this inserts $k$ immediately after $a$ in the cycle of $\sigma$: the arrows become $a\mapsto k\mapsto\sigma(a)$, with the other arrows unchanged.

Conversely, in any $k$-cycle there is a unique predecessor $a$ of $k$. Delete $k$ and join that predecessor to the successor of $k$; this uniquely recovers $\sigma$ and the factor $(a\ k)$. Hence every $k$-cycle occurs exactly once, and no other permutation occurs. Induction proves

$$
\boxed{\xi_k=X_2\cdots X_k=\sum_{\sigma\text{ a }k\text{-cycle in }S_k}\sigma}.
$$

Thus $\xi_k$ is a [conjugacy-class sum](../../../../../../../conjugacy-class-sum.md) in $\mathbb C S_k$, although it need not be central in $\mathbb C S_n$ when $k<n$.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 103](../../../../paper-103-split.md)
5. [Iii](../../../../split.md)
6. [2016](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
