<h1 id="5/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a finitely generated [associative algebra](../../../../../../associative-algebra-split.md) $A$, the [representation variety of an associative algebra](../../../../../../representation-variety-of-an-associative-algebra.md) consists of generator matrices satisfying all defining polynomial relations. With fixed orthogonal idempotents $1=\sum_{i=1}^me_i$, require a representation on $\bigoplus_i k^{n_i}$ to send $e_i$ to the standard vertex projector. This is the meaning of $\operatorname{Rep}_A(\mathbf n)$; without specified idempotents, use the usual single dimension $r$ and $\operatorname{Rep}_A(r)=\operatorname{Hom}_{k\text{-alg}}(A,M_r(k))$. Polynomial relations cut out a closed [affine variety](../../../../../../affine-algebraic-set.md) in the space of generator matrices.

The group $G=\prod_i\operatorname{GL}_{n_i}(k)$ acts by conjugation, preserving the prescribed projectors. Its stabilizer is $\operatorname{Aut}_A(X)$, a nonempty open subset of $\operatorname{End}_A(X)$. The [orbit dimension formula](../../../../../../orbit-dimension-formula.md) consequently gives

$$
\boxed{\dim G-\dim\mathcal O_X=\dim\operatorname{Stab}_G(x)=\dim\operatorname{Aut}_A(X)=\dim\operatorname{End}_A(X)}.
$$

A [degeneration of a module](../../../../../../degeneration-of-a-module.md) $X$ to $Y$ means that $\mathcal O_Y\subseteq\overline{\mathcal O_X}$, equivalently that one representative of $Y$ lies in this closure.

For $0\to X'\to X\to X''\to0$, choose a vector-space splitting, so every generator has block matrix $x_g=\left(\begin{smallmatrix}x'_g&b_g\\0&x''_g\end{smallmatrix}\right)$. Conjugation by $\operatorname{diag}(tI,I)$, $t\ne0$, gives

$$
x_g(t)=\begin{pmatrix}x'_g&t b_g\\0&x''_g\end{pmatrix}.
$$

This polynomial family extends to $t=0$, retains all algebra relations, and at zero represents $X'\oplus X''$. Thus [splitting an extension gives a module degeneration](../../../../../../split-extension-as-a-degeneration.md). Iterating along a [composition series](../../../../../../composition-series.md) gives **$X\rightsquigarrow\operatorname{gr}X=\bigoplus_jX_j/X_{j-1}$**. Degenerations are transitive because an orbit closure is closed and invariant under base change.

For the [one-arrow quiver](../../../../../../kronecker-quiver-with-one-arrow.md) with dimension vector $(n_1,n_2)$,

$$
\boxed{\operatorname{Rep}_Q(n_1,n_2)=\operatorname{Hom}_k(k^{n_1},k^{n_2})\cong M_{n_2\times n_1}(k)}.
$$

The action is $A\mapsto g_2Ag_1^{-1}$. Its [rank orbits of a matrix under left-right multiplication](../../../../../../rank-orbit-of-a-matrix-under-left-right-multiplication.md) are indexed by $r=0,\ldots,\min(n_1,n_2)$, with a representative containing an $r\times r$ identity block and zeros elsewhere. Their dimensions are $r(n_1+n_2-r)$; their closures contain exactly matrices of rank at most $r$.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [5](../../5.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
