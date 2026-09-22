# Singular value decomposition

↑ **Parent:** [Linear algebra](linear-algebra-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Singular_value_decomposition)

The [singular value decomposition](singular-value-decomposition.md) separates any [matrix](matrix.md) into input directions, stretching factors, and output directions. Every $m\times n$ complex [matrix](matrix.md) admits

$$
A=U\Sigma V^*,\qquad U\in\mathbb C^{m\times m},\quad
\Sigma\in\mathbb R^{m\times n},\quad V\in\mathbb C^{n\times n}.
$$

Here $U,V$ are [unitary matrices](unitary-matrix.md), $V^*=V^\dagger$ is the [conjugate transpose](conjugate-transpose.md), and $\Sigma$ is a rectangular [diagonal matrix](diagonal-matrix.md). Its $p=\min(m,n)$ diagonal entries are the [singular values](singular-value.md), ordered $\sigma_1\geq\cdots\geq\sigma_p\geq0$. We use the conventional letters: $V$ contains the [right singular vectors](right-singular-vector.md) $v_j$, while $U$ contains the [left singular vectors](left-singular-vector.md) $u_j$. Writing $A=V\Sigma U^\dagger$ instead merely swaps these two matrix names; it requires swapping their roles consistently. For real [matrices](matrix.md), choose [orthogonal matrices](orthogonal-matrix.md) and replace the [conjugate transpose](conjugate-transpose.md) with the [transpose](transpose.md).[Mazeika, The singular value decomposition and low rank approximation, §3](https://math.uchicago.edu/~may/REU2016/REUPapers/Mazeika.pdf)

Reading from right to left, $V^*$ expresses the input in an [orthonormal basis](orthonormal-basis.md), $\Sigma$ stretches or annihilates those coordinates, and $U$ assembles the output in another [orthonormal basis](orthonormal-basis.md). Unlike [matrix similarity](matrix-similarity.md), the input and output [bases](basis.md) can differ, and even have different sizes. A $3\times2$ [matrix](matrix.md) has full factors of sizes $3\times3$, $3\times2$, and $2\times2$. If its [matrix rank](matrix-rank.md) is $2$, one can retain only the active columns, giving sizes $3\times2$, $2\times2$, and $2\times2$ for $U_r,\Sigma_r,V_r^*$; the full $U$ additionally describes an unused output direction.

For a fully computed nonsymmetric example, take

$$
A=\begin{pmatrix}3&4\\-4/5&3/5\end{pmatrix},\qquad
U=I,\quad\Sigma=\begin{pmatrix}5&0\\0&1\end{pmatrix},\quad
V=\frac15\begin{pmatrix}3&-4\\4&3\end{pmatrix}.
$$

Multiplication gives $U\Sigma V^T=A$. The [right singular vectors](right-singular-vector.md) are $v_1=(3,4)^T/5$ and $v_2=(-4,3)^T/5$; their images are $Av_1=(5,0)^T$ and $Av_2=(0,1)^T$. Thus, parametrizing the [unit circle](complex-unit-circle.md) by $x=v_1\cos t+v_2\sin t$ gives $Ax=(5\cos t,\sin t)^T$. Its image is the [ellipse](ellipse.md) $y_1^2/25+y_2^2=1$. The two [singular values](singular-value.md) are its semiaxis lengths, and the [left singular vectors](left-singular-vector.md) point along its axes. The [singular value decomposition](singular-value-decomposition.md) finds precisely the perpendicular input directions whose images stay perpendicular.

<a id="image-the-unit-circle-becomes-an-ellipse-av-1-5u-1-and-av-2-u-2"></a>
![](singular-value-ellipse.png)

**[Figure 5](#image-the-unit-circle-becomes-an-ellipse-av-1-5u-1-and-av-2-u-2). The unit circle becomes an ellipse: $Av_1=5u_1$ and $Av_2=u_2$**.

For compression, write the [matrix](matrix.md) as a sum of [outer products](outer-product.md) and retain the largest terms:

$$
A=\sum_{j=1}^r\sigma_j u_jv_j^*,\qquad
A_k=\sum_{j=1}^k\sigma_j u_jv_j^*,\qquad
\|A-A_k\|_F^2=\sum_{j=k+1}^r\sigma_j^2,
$$

where $r$ is the [matrix rank](matrix-rank.md). Among all [matrices](matrix.md) of [matrix rank](matrix-rank.md) at most $k$, $A_k$ minimizes the [Frobenius norm](frobenius-norm.md) error; this is the [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md). The [operator norm](operator-norm.md) error is $\sigma_{k+1}$ for $k<r$. These statements concern specified [norms](norm.md), rather than guaranteeing that discarded details are visually or scientifically unimportant.[Mazeika, §4.3: low rank approximation](https://math.uchicago.edu/~may/REU2016/REUPapers/Mazeika.pdf)

Consider an $8\times10$ brightness [matrix](matrix.md) $B=pq^T+ab^T/2$, with

$$
p=(1,2,3,4,4,3,2,1)^T,\qquad q=(1,2,3,4,5,5,4,3,2,1)^T,
$$

and $a_i=(-1)^{i-1}$, $b_j=(-1)^{j-1}$. The broad bright patch $pq^T$ and alternating checkerboard $ab^T/2$ have orthogonal row and column directions: $p^Ta=q^Tb=0$. Their [singular values](singular-value.md) are $\sqrt{60\cdot110}=\sqrt{6600}$ and $\sqrt{8\cdot10}/2=\sqrt{20}$. This [low-rank approximation](low-rank-approximation.md) keeps the first [outer product](outer-product.md), giving $B_1=pq^T$, with [Frobenius norm](frobenius-norm.md) error $\sqrt{20}\approx4.472$ and relative error $\sqrt{20/6620}\approx5.50\%$. For example, $B_{11}=1.5$ becomes $1$, and $B_{12}=1.5$ becomes $2$: every entry changes by $0.5$ in magnitude. The discarded pattern is small but entirely lost.

<a id="image-an-8-times10-matrix-its-rank-one-approximation-and-the-discarded-checkerboard"></a>
![](singular-value-rank-one.png)

**[Figure 6](#image-an-8-times10-matrix-its-rank-one-approximation-and-the-discarded-checkerboard). An $8\times10$ matrix, its rank-one approximation, and the discarded checkerboard**.

For this illustrative [image compression](image-compression.md), storing one normalized [left singular vector](left-singular-vector.md), one normalized [right singular vector](right-singular-vector.md), and one [singular value](singular-value.md) requires $8+10+1=19$ scalars instead of $80$. This counts scalars at equal precision, before storage overhead. In general, $k(m+n+1)$ scalars beat $mn$ only for sufficiently small $k$, and small error requires a small discarded sum of squared [singular values](singular-value.md). The usefulness comes from measuring the tradeoff before throwing information away.[Verma, Singular value decomposition of real matrices, slides 9 and 15–16](https://math.mit.edu/~gs/linearalgebra/ila5/SVD_Slides.pdf)

**Table of contents**

- [Autonne-Takagi factorization](autonne-takagi-factorization.md)
- [Singular value](singular-value.md)
  - [Right singular vector](right-singular-vector.md)
  - [Left singular vector](left-singular-vector.md)

## ↑ Ancestors (5)

1. [Linear algebra](linear-algebra-split.md)
2. [Algebra](algebra-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (59)

- [Affine image of a circle](affine-image-of-a-circle.md)
- [Charged-lepton Yukawa matrix diagonalization](charged-lepton-yukawa-matrix-diagonalization.md)
- [Eckart-Young-Mirsky theorem](eckart-young-mirsky-theorem.md)
- [Gaussian posterior in the zero-noise limit](gaussian-posterior-in-the-zero-noise-limit.md)
- [Inverse problem](inverse-problem-split.md)
- [Low-rank approximation](low-rank-approximation.md)
- [Matrix decomposition](matrix-decomposition.md)
- [Moore-Penrose inverse](moore-penrose-inverse.md)
- [Normal equations for linear least squares](normal-equations-for-linear-least-squares.md)
- [Operator Schmidt rank](operator-schmidt-rank.md)
- [Overdetermined least-squares example](overdetermined-least-squares-example.md)
- [Solution](past-exam-of-the-gauge-field-theory-course-of-the-university-of-cambridge/2014/paper-1/3/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-25/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-30/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-66/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-49/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-37/3/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-23/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-45/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/3/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-48/3/a/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-65/5/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-69/3/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-111/4/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-323/4/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-331/4/b/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/ii/paper-4/21f/iii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-326/1/3/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-205/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-326/2/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-331/4/a/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/ib/paper-3/18h/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-323/1/a/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2021/iii/paper-326/1/1/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2022/iii/paper-326/1/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/ia/paper-1/7b/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-305/2/e/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2023/iii/paper-335/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2024/iii/paper-358/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-205/5/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2017/paper-1/18/d/solution.md)
- [Solution](past-exam-of-the-physics-of-the-earth-as-a-planet-course-of-the-university-of-cambridge/2015/paper-1/1/c/solution.md)
- [Solution](past-exam-of-the-quantum-information-course-of-the-university-of-cambridge/2016/paper-1/2/solution.md)
- [Principal component regression](principal-component-regression.md)
- [Ridge regression](ridge-regression.md)
- [Schmidt-rank contraction under product operators](schmidt-rank-contraction-under-product-operators.md)
- [Singular value](singular-value.md)
- [Singular value decomposition](singular-value-decomposition.md)
- [Small singular values in the Moore-Penrose inverse](small-singular-values-in-the-moore-penrose-inverse.md)
- [Tikhonov regularization](tikhonov-regularization.md)
- [Trace-class duality](trace-class-duality.md)
- [Truncated singular value decomposition](truncated-singular-value-decomposition.md)
- [Two-factor tensor rank](two-factor-tensor-rank.md)
- [Unitary polar factor of a finite compression](unitary-polar-factor-of-a-finite-compression.md)
- [Unitary variational formula for the trace norm](unitary-variational-formula-for-the-trace-norm.md)
