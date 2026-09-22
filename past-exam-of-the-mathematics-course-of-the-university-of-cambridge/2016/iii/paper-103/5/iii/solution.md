<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Assume $n\geq2$. The [standard Young tableaux](../../../../../../standard-young-tableau.md) of shape $(n-1,1)$ are $T_k$, for $2\leq k\leq n$: the sole second-row entry is $k$, and the first row is

$$
1,\ 2,\ldots,k-1,\ k+1,\ldots,n.
$$

This lists all of them, since $1$ must occupy the first box and the rest of the first row is forced to increase. Their contents are

$$
\boxed{
c_{T_k}(r)=
\begin{cases}
r-1,&r<k,\\
-1,&r=k,\\
r-2,&r>k.
\end{cases}}
$$

Write $w_k=w_{T_k}$. The only nontrivial adjacent swaps exchange the lower entry with $k-1$ or $k+1$. Substituting the content differences into [Young orthogonal form](../../../../../../young-orthogonal-form.md) yields **all generator actions**:

$$
\boxed{
s_jw_k=
\begin{cases}
-\dfrac1{k-1}w_k+\sqrt{1-\dfrac1{(k-1)^2}}\,w_{k-1},&j=k-1,\\[4pt]
\dfrac1k w_k+\sqrt{1-\dfrac1{k^2}}\,w_{k+1},&j=k,\\[4pt]
w_k,&j\notin\{k-1,k\}.
\end{cases}}
$$

In the first line at $k=2$, the square-root coefficient is zero and the action is $-w_2$, so no vector $w_1$ is needed. The second line is used only when $k<n$, since the generator $s_n$ does not exist.

The corresponding [Specht module](../../../../../../specht-module.md) is the sum-zero [standard representation of the symmetric group](../../../../../../standard-representation-of-the-symmetric-group.md):

$$
\boxed{S^{(n-1,1)}\cong\{(z_1,\ldots,z_n)\in\mathbb C^n:\sum z_i=0\}}.
$$

A concrete orthonormal realization is

$$
w_k=\frac{e_1+\cdots+e_{k-1}-(k-1)e_k}{\sqrt{k(k-1)}}.
$$

Permuting coordinates gives exactly the actions above, linking this orthogonal tableau basis with the [Gelfand–Tsetlin basis](../../../../../../gelfand-tsetlin-basis.md) found in Question 1. Here the printed $s_j$ are the adjacent Coxeter _generators_, rather than products of all generators.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 103](../../../paper-103-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
