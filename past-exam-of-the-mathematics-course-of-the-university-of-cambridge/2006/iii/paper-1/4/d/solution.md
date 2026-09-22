<h1 id="4/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

The displayed identity is valid for a [highest-weight vector](../../../../../../highest-weight-vector.md) $v$, satisfying $Xv=0$ and $Hv=kv$, not for arbitrary $v\in V$. For example, in the defining module with $k=1$, take $v=y$: then $XYv=0$ but the proposed right side for $n=1$ is $v\ne0$.

For a [highest-weight vector](../../../../../../highest-weight-vector.md), the [sl2 triple](../../../../../../sl2-triple.md) relations give $HY^jv=(k-2j)Y^jv$. The operator identity

$$
[X,Y^n]=\sum_{j=0}^{n-1}Y^jHY^{n-1-j}
$$

comes from expanding a [commutator](../../../../../../commutator.md) with a product. Apply it to $v$, using $Xv=0$. Each term becomes $(k-2(n-1-j))Y^{n-1}v$, so the sum is

$$
\boxed{XY^nv=n(k-n+1)Y^{n-1}v.}
$$

This proves the intended [sl2 highest-weight lowering formula](../../../../../../sl2-highest-weight-lowering-formula.md). The identity valid for an arbitrary vector is instead

$$
XY^nv=Y^nXv+nY^{n-1}(H-n+1)v.
$$

On the [basis](../../../../../../basis.md) $v,Yv,\ldots,Y^kv$ of the irreducible module, $XY$ has [eigenvalue](../../../../../../eigenvalue.md) $(j+1)(k-j)$ on $Y^jv$, for $0\leq j\leq k$. Summing gives the [trace of a raising-lowering product in an irreducible sl2 module](../../../../../../trace-of-a-raising-lowering-product-in-an-irreducible-sl2-module.md):

$$
\boxed{\operatorname{tr}_V(XY)=\sum_{j=0}^k(j+1)(k-j)=\frac{k(k+1)(k+2)}6.}
$$

The last equality follows by the formulas for the sums of the first $k$ integers and their squares.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
