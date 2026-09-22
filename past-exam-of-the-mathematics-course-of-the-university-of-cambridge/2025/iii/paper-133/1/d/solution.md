<h1 id="1/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Map both $a$ and $b$ to the nonidentity element of $C_2$. Both relators $a^2,b^2$ map to the identity, so this gives a homomorphism $D_\infty\to C_2$. A word of length $n$ maps to the parity class of $n$; consequently a null word has even length.

Now let $w$ be a null word of positive even length. Interpreting $a^{-1}=a$ and $b^{-1}=b$, the [free-product normal form theorem](../../../../../../normal-form-theorem-for-an-amalgamated-free-product.md) says that a nonempty alternating word cannot be trivial. Thus $w$ has two adjacent equal letters. Delete this $a^2$ or $b^2$, using one conjugate of a defining relator, and apply induction to the resulting null word of length $n-2$. This gives

$$
\boxed{\operatorname{Area}(w)\leq1+\frac{n-2}{2}=\frac n2.}
$$

## ↑ Ancestors (11)

1. [D](../d.md)
2. [1](../../1.md)
3. [Paper 133](../../../paper-133-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
