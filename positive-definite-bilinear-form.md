# Positive-definite bilinear form

↑ **Parent:** [Symmetric bilinear form](symmetric-bilinear-form.md)

A real [symmetric bilinear form](symmetric-bilinear-form.md) is [positive-definite](positive-definite-bilinear-form.md) when $B(v,v)>0$ for every nonzero [vector](vector.md). It defines an [inner product](inner-product.md) and the associated [norm](norm.md) $\sqrt{B(v,v)}$. Symmetry is part of this definition: positive diagonal values by themselves do not imply symmetry.[Alexei Skorobogatov, Linear Algebra and Matrices, pp. 13–14: positive forms and inner products](https://www.ma.imperial.ac.uk/~anskor/LINEAR.PDF)

The [identity matrix](identity-matrix.md) $A=\operatorname{diag}(1,1)$ gives $B(v,w)=v_1w_1+v_2w_2$ and $B(v,v)=v_1^2+v_2^2$. For $v=(3,4)$ this is $25$, giving [norm](norm.md) $5$. A weighted example, $A=\operatorname{diag}(4,1)$, gives [norm](norm.md) $\sqrt{4x^2+y^2}$: the first [coordinate](coordinate-linear-algebra.md) costs twice as much in length. Such [inner products](inner-product.md) let geometry assign different weights to different directions.

Every [positive-definite bilinear form](positive-definite-bilinear-form.md) is [nondegenerate](nondegenerate-bilinear-form.md): a [vector](vector.md) in its [radical of a bilinear form](radical-of-a-bilinear-form.md) has $B(v,v)=0$, so positivity forces $v=0$. The converse fails, as $\operatorname{diag}(1,-1)$ shows. Even positivity of the associated [quadratic form](quadratic-form.md) does not force a general [bilinear form](bilinear-form.md) to be symmetric: $A=\begin{pmatrix}1&1\\-1&1\end{pmatrix}$ has $v^TAv=x^2+y^2$ but $B(e_1,e_2)=1$ and $B(e_2,e_1)=-1$.

The complex [Killing form](killing-form.md) is not positive-definite on the entire complex [Cartan subalgebra](cartan-subalgebra.md); its restriction to the [Euclidean subspace of a Cartan subalgebra](euclidean-subspace-of-a-cartan-subalgebra.md) is a real positive-definite form.

**Table of contents**

- [Positive definiteness](positive-definiteness.md)
  - [Two-by-two positive-definiteness test](two-by-two-positive-definiteness-test.md)
  - [Positive-definiteness threshold in a two-by-two family](positive-definiteness-threshold-in-a-two-by-two-family.md)
  - [Ellipsoid level sets of a positive-definite quadratic form](ellipsoid-level-sets-of-a-positive-definite-quadratic-form.md)
  - [Unique minimizer of a positive-definite quadratic function](unique-minimizer-of-a-positive-definite-quadratic-function.md)

## ↑ Ancestors (7)

1. [Symmetric bilinear form](symmetric-bilinear-form.md)
2. [Bilinear form](bilinear-form.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Minkowski metric](minkowski-metric.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2011/ii/paper-4/19i/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-19/4/solution.md)
- [Positive-definite bilinear form](positive-definite-bilinear-form.md)
- [Symmetric bilinear form](symmetric-bilinear-form.md)
