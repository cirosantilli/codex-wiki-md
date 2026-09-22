# Singular matrix

↑ **Parent:** [Invertible matrix](invertible-matrix.md)

An $n\times n$ [square matrix](square-matrix.md) $A$ over a [field](field.md), with $n\geq1$, is singular when it has no [matrix inverse](matrix-inverse-split.md). Geometrically, its [linear map](linear-map.md) loses at least one input direction: some nonzero [vector](vector.md) $v$ satisfies $Av=0$, so $A(x+v)=Ax$. Over the [real numbers](real-number.md), the following family makes that loss visible:

$$
A(t)=\begin{pmatrix}1&0\\0&t\end{pmatrix},\qquad A(t)(x,y)=(x,ty).
$$

<a id="image-compression-by-a-t-operatorname-diag-1-t-becomes-collapse-only-at-t-0"></a>
![](singularity-nullity-collapse.png)

**[Figure 16](#image-compression-by-a-t-operatorname-diag-1-t-becomes-collapse-only-at-t-0). Compression by $A(t)=\operatorname{diag}(1,t)$ becomes collapse only at $t=0$**. The [square](square.md) $[-1,1]^2$ retains two-dimensional extent for $t=1$ and $t=0.15$, but maps to a segment at $t=0$. The orange points come from three inputs with the same first coordinate and different second coordinates. They coincide only at $t=0$. This is exact illustrative geometry, not measured data.

For this [diagonal matrix](diagonal-matrix.md), $\det A(t)=t$. Whenever $t\ne0$, the input can be recovered as $(x,y)=(b_1,b_2/t)$ and the [kernel](kernel-of-a-linear-map-split.md) is $\{0\}$. At $t=0$, the [kernel](kernel-of-a-linear-map-split.md) becomes $\operatorname{span}\{(0,1)\}$: the entire second coordinate is forgotten. Consequently $A(0)x=(b_1,b_2)$ has no solution if $b_2\ne0$, and has the solution [straight line](straight-line.md) $x=(b_1,s)$, $s\in\mathbb R$, if $b_2=0$. A [singular matrix](singular-matrix.md) therefore need not make a particular [linear system](system-of-linear-equations.md) inconsistent; it prevents unique recovery when that [linear system](system-of-linear-equations.md) is consistent.

For an $n\times n$ [square matrix](square-matrix.md), all these tests describe the same failure:

$$
\boxed{
A\text{ singular}
\iff\det A=0
\iff\operatorname{rank}A<n
\iff\ker A\ne\{0\}
\iff\operatorname{im}A\ne\mathbb F^n.
}
$$

Here $\mathbb F$ is the [field](field.md) of [scalars](scalar.md). Equivalently, the columns are [linearly dependent](linear-dependence.md), the [linear map](linear-map.md) is neither [injective](injective-function.md) nor [surjective](surjective-function.md), and some outputs cannot be reached. See the [invertible matrix](invertible-matrix.md) equivalences and [Strang's MIT 18.06SC lecture summary, Multiplication and inverse matrices, p. 2](https://www.ocw.mit.edu/courses/18-06sc-linear-algebra-fall-2011/1963da71c4d96e5d14e7939780f79bcc_MIT18_06SCF11_Ses1.3sum.pdf). Over an infinite [field](field.md), every consistent [linear system](system-of-linear-equations.md) for a [singular matrix](singular-matrix.md) has infinitely many solutions; over a finite [field](field.md) with $q$ elements and [nullity](nullity-of-a-linear-map.md) $d$, it has exactly $q^d$ solutions. This follows by adding each [kernel](kernel-of-a-linear-map-split.md) [vector](vector.md) to one solution.

The square hypothesis is essential. For an $m\times n$ [matrix](matrix.md), [injectivity](injective-function.md) means [matrix rank](matrix-rank.md) $n$ ([full column rank](full-column-rank.md)), whereas [surjectivity](surjective-function.md) means [matrix rank](matrix-rank.md) $m$ ([full row rank](full-row-rank.md)). A rectangular [matrix](matrix.md) can satisfy one condition without the other; its [kernel](kernel-of-a-linear-map-split.md) and [image of a linear map](image-of-a-linear-map.md) give the useful tests without calling it a [singular matrix](singular-matrix.md).

Exact singularity also differs from sensitivity. For $0<|t|\leq1$, $A(t)$ is an [invertible matrix](invertible-matrix.md), but its smallest [singular value](singular-value.md) is $|t|$ and its [condition number](condition-number.md) in [Euclidean norm](euclidean-norm.md) is $1/|t|$. A change $\delta b=(0,\varepsilon)$ changes the recovered input by $\delta x=(0,\varepsilon/t)$: with $t=1/100$ and $\varepsilon=1/1000$, an output change of $0.001$ causes an input change of $0.1$. These are exact toy values, not measurements. The [condition number](condition-number.md) quantifies this sensitivity before a direction is lost; see [Steve Marschner, Condition numbers, §2](https://www.cs.cornell.edu/courses/cs322/2007sp/notes/condition.pdf). A small [determinant](determinant.md) alone is not a reliable sensitivity test: $\varepsilon I_2$ has [determinant](determinant.md) $\varepsilon^2$ yet [condition number](condition-number.md) one for every nonzero real $\varepsilon$, since both [singular values](singular-value.md) shrink equally.

**Table of contents**

- [Singularity forced by an odd-dimensional transpose-inverse identity](singularity-forced-by-an-odd-dimensional-transpose-inverse-identity.md)

## ↑ Ancestors (6)

1. [Invertible matrix](invertible-matrix.md)
2. [Linear algebra](linear-algebra-split.md)
3. [Algebra](algebra-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (19)

- [Choosing a different block pivot](choosing-a-different-block-pivot.md)
- [Degenerate conic](degenerate-conic.md)
- [Determinant](determinant.md)
- [Gaussian elimination with a row swap](gaussian-elimination-with-a-row-swap.md)
- [Gaussian filtering with exact observations](gaussian-filtering-with-exact-observations.md)
- [Matrix inverse](matrix-inverse-split.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/ib/paper-1/1e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2019/ib/paper-2/10f/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2008/paper-1/18/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/14/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2011/paper-2/14/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2012/paper-1/11/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge/2024/paper-1/5/b/solution.md)
- [Pivoted LU decomposition](pivoted-lu-decomposition.md)
- [Rank-one update singularity criterion](rank-one-update-singularity-criterion.md)
- [Schur complement determinant identity](schur-complement-determinant-identity.md)
- [Singular matrix](singular-matrix.md)
- [Singularity forced by an odd-dimensional transpose-inverse identity](singularity-forced-by-an-odd-dimensional-transpose-inverse-identity.md)
- [Trivial kernel](trivial-kernel.md)
