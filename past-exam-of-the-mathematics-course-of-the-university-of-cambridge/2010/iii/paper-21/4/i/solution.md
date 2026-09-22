<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $U_n:\mathcal C_{n+1}\to\mathcal C_n$ forget the last [partial unary operation](../../../../../../partial-unary-operation.md). For an object $A$ of the [nested partial unary operation category](../../../../../../nested-partial-unary-operation-category.md) $\mathcal C_n$, set

$$
S_n(A)=\{x\in A:\alpha_n(x)\text{ is defined and }\alpha_n(x)=x\}.
$$

The nesting rule implies that every earlier operation is defined and fixes such an $x$. To construct a [free extension of nested partial unary operations](../../../../../../free-extension-of-nested-partial-unary-operations.md), adjoin a disjoint infinite chain for each $x\in S_n(A)$:

$$
L_nA=A\amalg\{(x,k):x\in S_n(A),\ k\in\mathbb N\}.
$$

Keep the old operations on $A$. On each new chain put $\alpha_1(x,k)=(x,k+1)$; every old operation $\alpha_i$ with $2\leq i\leq n$ is undefined there, because the first operation has no fixed points there. Define the new operation only on $S_n(A)$, by $\alpha_{n+1}(x)=(x,0)$. These are exactly the fixed points of the old top operation, so the required domain rule is satisfied. The inclusion $A\hookrightarrow U_nL_nA$ preserves all old defined operations.

For a [morphism](../../../../../../morphism.md) $f:A\to U_nB$, preservation of the old operations makes $f(x)\in S_n(B)$ whenever $x\in S_n(A)$. Any extension to a morphism $\widehat f:L_nA\to B$ must have

$$
\widehat f(x,k)=\beta_1^k\bigl(\beta_{n+1}(f(x))\bigr),\qquad \widehat f|_A=f.
$$

The operation $\beta_{n+1}$ is defined at $f(x)$, and $\beta_1$ is total, so this formula exists. It preserves the new operation and the chain operation; there are no other defined operations on new points to check. It therefore gives the unique extension. Naturality and functoriality follow from uniqueness. Thus

$$
\boxed{\mathcal C_{n+1}(L_nA,B)\cong\mathcal C_n(A,U_nB),\qquad L_n\dashv U_n.}
$$

Notice the useful extra fact: the new top operation has no fixed points, since every value $(x,0)$ is new and every input $x$ is old. Hence freely adding any further operations adds no more points; those operations have empty domains.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
