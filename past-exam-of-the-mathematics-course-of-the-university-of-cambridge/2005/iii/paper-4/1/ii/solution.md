<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

We construct a [Hermitian hyperbolic plane over a finite field](../../../../../../hermitian-hyperbolic-plane-over-a-finite-field.md) inside each successive two-dimensional piece. By the [field norm](../../../../../../field-norm.md) surjectivity proved above, choose $a\in\mathbb F_{q^2}$ with $a\bar a=-1$. From two vectors in an [orthonormal basis](../../../../../../orthonormal-basis.md), form $e=v_1+av_2$. Then $B(e,e)=1+a\bar a=0$, so $e$ is a nonzero [isotropic vector](../../../../../../isotropic-vector.md). Nondegeneracy supplies $g$ with $B(e,g)=1$; rescaling the second argument achieves this normalization. In fact $g=v_1$ already works in this two-dimensional piece. By [quadratic finite-field norm and trace surjectivity](../../../../../../quadratic-finite-field-norm-and-trace-surjectivity.md), choose $c$ with $c+\bar c=B(g,g)$ and put $f=g-ce$. Direct expansion gives

$$
B(e,f)=1,\qquad B(f,f)=B(g,g)-c-\bar c=0.
$$

Thus $e,f$ are [linearly independent](../../../../../../linear-independence.md), and their [Gram matrix](../../../../../../gram-matrix.md) is $\begin{pmatrix}0&1\\1&0\end{pmatrix}$, which is invertible even in characteristic two. Their span is nondegenerate, so its [orthogonal complement for a sesquilinear form](../../../../../../orthogonal-complement-for-a-sesquilinear-form.md) is again nondegenerate. Repeat the construction there. In even dimension this exhausts $V$; in odd dimension the final one-dimensional complement has a nonzero diagonal value, which can be normalized to one using the [field norm](../../../../../../field-norm.md). Calling its vector $d$, we obtain

$$
\boxed{B(e_i,f_j)=\delta_{ij},\quad B(e_i,e_j)=B(f_i,f_j)=0,\quad B(d,d)=1,\quad B(d,e_i)=B(d,f_i)=0,}
$$

with the $d$ terms present only in odd dimension. This proves all the requested pairings and the [basis](../../../../../../basis.md) assertion.

The printed hint needs a qualification. If $X^2-X-1$ is irreducible over $\mathbb F_q$, its two roots are conjugate, so $\zeta+\bar\zeta=1$ and $\zeta\bar\zeta=-1$; the hinted vectors then do work. They need not work when it splits. For example, over $\mathbb F_{11}$ its roots are $4,8$, fixed by conjugation in $\mathbb F_{121}$. For either choice the proposed $e$ has norm $1+\zeta^2$, respectively $6$ or $10$, rather than zero. The norm-and-trace construction above proves the assertion without that restriction.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
