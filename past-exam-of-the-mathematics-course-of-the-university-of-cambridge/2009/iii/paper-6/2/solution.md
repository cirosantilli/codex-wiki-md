<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $B$ be the given [invariant bilinear form on a Lie algebra](../../../../../invariant-bilinear-form-on-a-lie-algebra.md). Choose a [basis](../../../../../basis.md) $x_1,\ldots,x_d$ and its $B$-dual [basis](../../../../../basis.md) $x^1,\ldots,x^d$, so $B(x_i,x^j)=\delta_i^j$. The [Casimir element](../../../../../casimir-element.md) is

$$
\boxed{\Omega_B=\sum_i x_i x^i\in U(\mathfrak g).}
$$

The tensor $\sum_i x_i\otimes x^i$ is the inverse tensor of $B$, so it is independent of the chosen [basis](../../../../../basis.md). Multiplication in the [universal enveloping algebra](../../../../../universal-enveloping-algebra.md) therefore makes $\Omega_B$ independent of that choice as well.

For $z\in\mathfrak g$, write $[z,x_i]=\sum_j a_{ji}x_j$. Invariance means $B([z,x],y)+B(x,[z,y])=0$, whence $[z,x^i]=-\sum_j a_{ij}x^j$. Therefore

$$
[z,\Omega_B]=\sum_{i,j}a_{ji}x_jx^i-\sum_{i,j}a_{ij}x_ix^j=0,
$$

by interchanging $i,j$ in the second sum. Since $\mathfrak g$ generates its [universal enveloping algebra](../../../../../universal-enveloping-algebra.md), $\Omega_B$ is central. This argument does not require adding a symmetry assumption to the given [bilinear form](../../../../../bilinear-form.md).

For the [sl2 Lie algebra](../../../../../sl2-lie-algebra.md), take

$$
e=\begin{pmatrix}0&1\\0&0\end{pmatrix},\quad f=\begin{pmatrix}0&0\\1&0\end{pmatrix},\quad h=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad B(X,Y)=\operatorname{tr}(XY).
$$

The cyclic identity for the [trace](../../../../../matrix-trace.md) gives $B([Z,X],Y)+B(X,[Z,Y])=0$. The form is [nondegenerate](../../../../../nondegenerate-bilinear-form.md), since $B(e,f)=1$, $B(h,h)=2$, and all the other pairings except $B(f,e)$ are zero. The dual of $(e,f,h)$ is $(f,e,h/2)$, so

$$
\Omega_B=ef+fe+\tfrac12h^2.
$$

By the [classification of finite-dimensional sl2 representations](../../../../../classification-of-finite-dimensional-sl2-representations.md), an irreducible of [dimension](../../../../../dimension-vector-space.md) $n$ has a [highest-weight vector](../../../../../highest-weight-vector.md) $v$ with $ev=0$ and $hv=mv$, where $m=n-1$. Since $ef=fe+h$, one obtains

$$
\Omega_Bv=\left(m+\tfrac12m^2\right)v.
$$

Centrality and the [Schur lemma](../../../../../schur-s-lemma.md) then give the answer on the entire representation:

$$
\boxed{\Omega_B=\frac{n^2-1}{2}I.}
$$

This [Casimir eigenvalue for sl2](../../../../../casimir-eigenvalue-for-sl2.md) depends on normalization. Choosing the [Killing form](../../../../../killing-form.md) instead, $K=4B$, scales the dual [basis](../../../../../basis.md) and the [Casimir element](../../../../../casimir-element.md) by $1/4$, giving $(n^2-1)I/8$.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 6](../../paper-6-split.md)
3. [Iii](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
