# Alternating bilinear form

↑ **Parent:** [Bilinear form](bilinear-form-split.md)

A [bilinear form](bilinear-form-split.md) is alternating if $B(v,v)=0$ for every [vector](vector.md) $v$. Expanding $B(v+w,v+w)=0$ gives $B(v,w)+B(w,v)=0$, hence $B(v,w)=-B(w,v)$. If the [characteristic](characteristic-of-a-field.md) is not two, the converse follows from $B(v,v)=-B(v,v)$ by dividing by two. In [characteristic](characteristic-of-a-field.md) two, the relation $B(v,w)=-B(w,v)$ is just symmetry and does not force zero self-pairings: $B(x,y)=xy$ on $\mathbb F_2$ has $B(1,1)=1$.[Peter J. Cameron, Notes on Linear Algebra, §§9.1–9.2: alternating forms in arbitrary characteristic](https://webspace.maths.qmul.ac.uk/p.j.cameron/notes/linalg.pdf)

The [matrix](matrix.md)

$$
J=\begin{pmatrix}0&1\\-1&0\end{pmatrix},\qquad B(v,w)=v^TJw=v_1w_2-v_2w_1=\det\begin{pmatrix}v_1&w_1\\v_2&w_2\end{pmatrix}
$$

gives an [alternating bilinear form](alternating-bilinear-form.md) over every [field](field.md). Over the [real numbers](real-number.md), its value is the signed [area](surface-area.md) of the [parallelogram](parallelogram.md) with sides $v,w$: $B((2,1),(1,3))=6-1=5$, and swapping the sides gives $-5$. Every self-pairing is zero, yet $\det J=1$, so this [bilinear form](bilinear-form-split.md) is [nondegenerate](nondegenerate-bilinear-form.md). Directly, pairing $(x,y)$ with $(1,0)$ gives $-y$, and pairing it with $(0,1)$ gives $x$; both vanish only when $(x,y)=0$.

In [characteristic](characteristic-of-a-field.md) different from two, a [skew-symmetric matrix](skew-symmetric-matrix.md) of [odd integer](odd-integer.md) size has zero [determinant](determinant.md), since $\det A=\det(-A^T)=(-1)^n\det A$. Thus an [alternating bilinear form](alternating-bilinear-form.md) on a finite odd-dimensional [vector space](vector-space-split.md) is a [degenerate bilinear form](degenerate-bilinear-form.md). The stronger statement that the [rank](rank-one-quadratic-form.md) of an [alternating bilinear form](alternating-bilinear-form.md) is even holds in all [characteristics](characteristic-of-a-field.md): splitting off a two-dimensional block with [matrix](matrix.md) $J$ repeatedly proves it. A [nondegenerate](nondegenerate-bilinear-form.md) [alternating bilinear form](alternating-bilinear-form.md) defines a [symplectic vector space](symplectic-vector-space.md), the linear setting for signed [area](surface-area.md) rather than squared length.

## ↑ Ancestors (6)

1. [Bilinear form](bilinear-form-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (46)

- [Alternating bilinear form](alternating-bilinear-form.md)
- [Anisotropic vector for a form](anisotropic-vector-for-a-form.md)
- [Bilinear form](bilinear-form-split.md)
- [Binary quadratic refinement](binary-quadratic-refinement.md)
- [Degenerate bilinear form](degenerate-bilinear-form.md)
- [Euler characteristic parity in dimensions congruent to two modulo four](euler-characteristic-parity-in-dimensions-congruent-to-two-modulo-four.md)
- [Exterior and symmetric squares of the seven-dimensional G2 representation](exterior-and-symmetric-squares-of-the-seven-dimensional-g2-representation.md)
- [Four-dimensional symplectic basis change](four-dimensional-symplectic-basis-change.md)
- [Hyperbolic pair](hyperbolic-pair.md)
- [Invariant form on an irreducible sl2 module](invariant-form-on-an-irreducible-sl2-module.md)
- [Lie-invariant bilinear form](lie-invariant-bilinear-form.md)
- [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
- [Orthogonal group over a finite field](orthogonal-group-over-a-finite-field.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-3/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-16/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-2/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/4/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-4/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-3/3/c/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-12/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-114/5/solution.md)
- [Polar bilinear form of a quadratic form](polar-bilinear-form-of-a-quadratic-form.md)
- [Quadratic form](quadratic-form-split.md)
- [Radical of a bilinear form](radical-of-a-bilinear-form.md)
- [Right radical of a bilinear form](right-radical-of-a-bilinear-form.md)
- [Symmetric and alternating parts of a bilinear form](symmetric-and-alternating-parts-of-a-bilinear-form.md)
- [Symplectic basis](symplectic-basis.md)
- [Symplectic group over a field](symplectic-group-over-a-field.md)
- [Symplectic group over a finite field](symplectic-group-over-a-finite-field.md)
- [Symplectic quotient of the binary subset module](symplectic-quotient-of-the-binary-subset-module.md)
- [Symplectic vector space](symplectic-vector-space.md)
- [Transvection](transvection.md)
- [Witt's theorem](witt-s-theorem.md)
