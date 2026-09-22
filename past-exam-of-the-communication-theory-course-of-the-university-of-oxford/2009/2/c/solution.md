<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Suppose every sum of two distinct probabilities exceeds every third [probability](../../../../probability.md). If an optimal code were not a [block code](../../../../block-code.md), part (b) gives two deepest sibling leaves $x,y$ at depth $L>n$ and a leaf $z$ at depth $\ell<n$. Replace the sibling pair by a leaf labelled $z$, and replace the former $z$ leaf by two children labelled $x,y$. The resulting tree is still a prefix tree, and other word lengths are unchanged. The change in expected length is

$$
(p_x+p_y)(\ell+1-L)+p_z(L-1-\ell)
=(L-\ell-1)(p_z-p_x-p_y)<0.
$$

Here $L-\ell-1\geq1$. This contradicts optimality. Thus **every optimal code is a [block code](../../../../block-code.md)**.

Conversely, suppose distinct $x,y,z$ satisfy $p_x+p_y\leq p_z$. Starting with the complete length-$n$ code, arrange $x,y$ as a sibling pair, which is possible by permuting the source labels. Its parent at depth $n-1$ does not contain $z$. Label that parent $z$, and split the old $z$ leaf into children $x,y$. This gives lengths $n-1$ for $z$, $n+1$ for $x,y$, and $n$ otherwise, with expected length

$$
n+p_x+p_y-p_z\leq n.
$$

If the optimal mean length is below $n$, no optimal code can be a [block code](../../../../block-code.md): any injective binary [block code](../../../../block-code.md) for $2^n$ symbols has length at least $n$. If the optimal mean is $n$, the constructed non-[block code](../../../../block-code.md) itself is optimal. In either case there is an optimal non-[block code](../../../../block-code.md). This proves the reverse implication, including the equality case, and hence the **strict** inequality in the criterion is necessary.

This is the [optimality of a fixed-length code for a power-of-two alphabet](../../../../optimality-of-a-fixed-length-code-for-a-power-of-two-alphabet.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
