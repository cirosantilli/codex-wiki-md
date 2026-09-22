# Symmetric bilinear form

↑ **Parent:** [Bilinear form](bilinear-form-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Symmetric_bilinear_form)

A [bilinear form](bilinear-form-split.md) $B$ is symmetric when $B(v,w)=B(w,v)$ for every pair of [vectors](vector.md) $v,w$. Equivalently, its [matrix of a bilinear form](matrix-of-a-bilinear-form.md) in any [basis](basis.md) is a [symmetric matrix](symmetric-matrix.md), since $A_{ij}=B(e_i,e_j)=B(e_j,e_i)=A_{ji}$. Symmetry makes the relation $B(v,w)=0$ reciprocal, giving the [bilinear orthogonal complement](orthogonal-complement-for-a-bilinear-form.md) a geometric interpretation.

Over the [real numbers](real-number.md), set $q(v)=B(v,v)$. The [polarization identity](polarization-identity.md)

$$
B(v,w)=\frac12\bigl(q(v+w)-q(v)-q(w)\bigr)
$$

recovers the [symmetric bilinear form](symmetric-bilinear-form.md) from its [quadratic form](quadratic-form-split.md): expand $q(v+w)$ and use symmetry to combine the two cross terms. For $q(x,y)=x^2-y^2$, take $v=(2,1)$ and $w=(1,3)$. Then $q(v+w)=-7$, $q(v)=3$, and $q(w)=-8$, so $B(v,w)=(-7-3+8)/2=-1=2\cdot1-1\cdot3$. The same formula works whenever the [characteristic](characteristic-of-a-field.md) is not two.[Skorobogatov, Linear Algebra and Matrices, p. 12: recovering a symmetric form from the diagonal](https://www.ma.imperial.ac.uk/~anskor/LINEAR.PDF)

Three real [diagonal matrices](diagonal-matrix.md) show how much variety symmetry allows. The [identity matrix](identity-matrix.md) $\operatorname{diag}(1,1)$ gives the [positive-definite bilinear form](positive-definite-bilinear-form.md) $q=x^2+y^2$. The [matrix](matrix.md) $\operatorname{diag}(1,-1)$ gives $q=x^2-y^2$ and is [nondegenerate](nondegenerate-bilinear-form.md) despite the [isotropic vector](isotropic-vector.md) $(1,1)$. The [matrix](matrix.md) $\operatorname{diag}(1,0)$ gives $q=x^2$ and is a [degenerate bilinear form](degenerate-bilinear-form.md) with [radical of a bilinear form](radical-of-a-bilinear-form.md) $\operatorname{span}\{(0,1)\}$. Their [level sets](level-set.md) make the distinction visible: a [circle](circle.md), two branches of a [hyperbola](hyperbola.md), and two parallel lines for $q=1$.

<a id="image-unit-and-zero-level-sets-distinguish-positive-indefinite-nondegenerate-and-degenerate-symmetric-forms"></a>
![](quadratic-form-level-sets.png)

**[Figure 2](#image-unit-and-zero-level-sets-distinguish-positive-indefinite-nondegenerate-and-degenerate-symmetric-forms). Unit and zero level sets distinguish positive, indefinite nondegenerate, and degenerate symmetric forms**.

The [inertia of a bilinear form](inertia-of-a-bilinear-form.md) records the numbers of positive, negative, and zero directions after [matrix congruence](matrix-congruence.md) diagonalization. By [Sylvester's law of inertia](sylvester-s-law-of-inertia.md), these counts survive [change of basis](change-of-basis.md); the three examples have [inertia of a bilinear form](inertia-of-a-bilinear-form.md) $(2,0,0)$, $(1,1,0)$, and $(1,0,1)$. Historically, Sylvester stated this invariance in an 1852 paper on reducing real [quadratic forms](quadratic-form-split.md) to sums of positive and negative squares. Ghys and Ranicki reproduce his statement and distinguish it from his subsequent 1853 proof.[Étienne Ghys and Andrew Ranicki, Signatures in algebra, topology and dynamics, §1.2: Sylvester's statement and proof](https://arxiv.org/pdf/1512.09258)

**Table of contents**

- [Positive-definite bilinear form](positive-definite-bilinear-form.md)
  - [Positive definiteness](positive-definiteness.md)
    - [Two-by-two positive-definiteness test](two-by-two-positive-definiteness-test.md)
    - [Positive-definiteness threshold in a two-by-two family](positive-definiteness-threshold-in-a-two-by-two-family.md)
    - [Ellipsoid level sets of a positive-definite quadratic form](ellipsoid-level-sets-of-a-positive-definite-quadratic-form.md)
    - [Unique minimizer of a positive-definite quadratic function](unique-minimizer-of-a-positive-definite-quadratic-function.md)
- [Modified trace form on real matrices](modified-trace-form-on-real-matrices.md)
- [Witt group of a field](witt-group-of-a-field.md)

## ↑ Ancestors (6)

1. [Bilinear form](bilinear-form-split.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (55)

- [Alternating trilinear form](alternating-trilinear-form.md)
- [Anisotropic vector for a form](anisotropic-vector-for-a-form.md)
- [Bilinear form](bilinear-form-split.md)
- [Bilinearity](bilinearity.md)
- [Bounded bilinear form](bounded-bilinear-form.md)
- [Coercive bilinear form](coercive-bilinear-form.md)
- [Degenerate bilinear form](degenerate-bilinear-form.md)
- [Degenerate metric tensor](degenerate-metric-tensor.md)
- [Exceptional isomorphism between sp4 and so5](exceptional-isomorphism-between-sp4-and-so5.md)
- [Exterior square of the defining orthogonal representation](exterior-square-of-the-defining-orthogonal-representation.md)
- [Invariant form on an irreducible sl2 module](invariant-form-on-an-irreducible-sl2-module.md)
- [Lie-invariant bilinear form](lie-invariant-bilinear-form.md)
- [Matrix of a bilinear form](matrix-of-a-bilinear-form.md)
- [Minkowski metric](minkowski-metric.md)
- [Modified trace form on real matrices](modified-trace-form-on-real-matrices.md)
- [Nondegenerate bilinear form](nondegenerate-bilinear-form.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/ib/paper-1/17b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-62/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/ib/paper-1/8f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-4/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-2/12e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-2/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3/1/iii/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-3/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-2/5/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-19/5/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-68/4/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ii/paper-1/19g/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-17/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-45/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-59/1/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-6/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-1/4/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-1/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-15/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-66/7/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-205/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-302/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ib/paper-4/1f/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/2/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/2/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-102/3/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-102/3/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-105/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/iii/paper-102/1/c/solution.md)
- [Positive-definite bilinear form](positive-definite-bilinear-form.md)
- [Primitive exterior square](primitive-exterior-square.md)
- [Radical of a bilinear form](radical-of-a-bilinear-form.md)
- [Right radical of a bilinear form](right-radical-of-a-bilinear-form.md)
- [Signature pair of a real symmetric bilinear form](signature-pair-of-a-real-symmetric-bilinear-form.md)
- [Symmetric and alternating parts of a bilinear form](symmetric-and-alternating-parts-of-a-bilinear-form.md)
- [Symmetric bilinear form](symmetric-bilinear-form.md)
- [Symplectic basis](symplectic-basis.md)
- [Traceless symmetric square of the defining even orthogonal representation](traceless-symmetric-square-of-the-defining-even-orthogonal-representation.md)
- [Witt's theorem](witt-s-theorem.md)
