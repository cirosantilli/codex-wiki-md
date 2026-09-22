<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

An embedding is determined by its chosen increasing sequence of positions. Accordingly, the [all-subsequence embedding kernel](../../../../../all-subsequence-embedding-kernel.md) $K(x,y)$ counts pairs of embeddings, one in $x$ and one in $y$, that spell the same [subsequence](../../../../../subsequence.md). The two embeddings are distinguished even when they spell the same word as another pair. The empty word contributes exactly one pair.

Let $n=|x|$, $p=|y|$, and define $F(i,j)=K(x_1\cdots x_i,y_1\cdots y_j)$ for prefixes. When either prefix is empty, only the empty word has an embedding in both, so

$$
F(0,j)=F(i,0)=1.
$$

To derive a [dynamic programming recurrence](../../../../../dynamic-programming-recurrence.md), count pairs that do not use position $i$ of $x$ or do not use position $j$ of $y$. [Inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) gives

$$
F(i-1,j)+F(i,j-1)-F(i-1,j-1).
$$

The remaining pairs use both final positions. These positions must be the final letters of the common word, so they contribute nothing if $x_i\ne y_j$. If $x_i=y_j$, deleting those two final positions is a [bijection](../../../../../bijection.md) to arbitrary embedding pairs on the two shorter prefixes, including their empty pair. Their contribution is therefore $F(i-1,j-1)$. Hence

$$
\boxed{F(i,j)=F(i-1,j)+F(i,j-1)-F(i-1,j-1)
+\mathbf1_{\{x_i=y_j\}}F(i-1,j-1).}
$$

Equivalently, when the final symbols agree the recurrence simplifies to $F(i,j)=F(i-1,j)+F(i,j-1)$; when they differ, subtract the diagonal term. Fill the table in increasing prefix order and return $F(n,p)$. The boundary values and the disjoint counting argument prove correctness by [induction](../../../../../mathematical-induction.md) on $i+j$.

A one-row implementation of this [dynamic programming](../../../../../dynamic-programming.md) uses the saved old diagonal entry:
```
F[0..p] := 1
for i := 1 to n:
    diagonal := 1
    for j := 1 to p:
        above := F[j]
        if x[i] = y[j]:
            F[j] := above + F[j-1]
        else:
            F[j] := above + F[j-1] - diagonal
        diagonal := above
return F[p]
```
The assignment to `diagonal` retains the value from the previous row before `F[j]` was overwritten. Swapping $x$ and $y$ if necessary minimizes the row length. Thus the [time complexity](../../../../../time-complexity.md) is **$O(|x||y|)$ arithmetic operations** and the extra [space complexity](../../../../../space-complexity.md) is **$O(\min(|x|,|y|))$ integer cells**. Empty inputs return one immediately.

These counts include multiplicity: for $x=y=aa$, the empty word contributes $1$, the word $a$ contributes $2\cdot2=4$, and $aa$ contributes $1$, giving $K(aa,aa)=6$, not three. More generally, each result is at most $2^{n+p}$, since it counts some pairs of position subsets. Exact integers therefore require $O(n+p)$ bits; the stated quadratic bound is an arithmetic-operation bound, with a conservative $O(np(n+p))$ bound for elementary bit arithmetic.

The proposed [positive-semidefinite kernel](../../../../../positive-semidefinite-kernel-split.md) is valid: for each finite string only finitely many coordinates $\phi_u(x)$ are nonzero, so $x\mapsto(\phi_u(x))_{u\in\Delta^*}$ is a well-defined [feature map](../../../../../feature-map.md) into the [inner product space](../../../../../inner-product-space.md) of finitely supported coordinate families, and its [inner product](../../../../../inner-product-split.md) is exactly $K$.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Computational learning theory](../../../computational-learning-theory-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
