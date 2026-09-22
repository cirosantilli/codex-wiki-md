<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

**Nilpotence and eigenvalues.** If $Av=\lambda v$ with $v\ne0$, then $A^nv=\lambda^nv$. Thus $A^n=0$ forces $\lambda=0$ for every [eigenvalue](../../../../eigenvalue.md). Conversely, if all $n$ complex [eigenvalues](../../../../eigenvalue.md), counted with [algebraic multiplicity](../../../../algebraic-multiplicity.md), vanish, the monic [characteristic polynomial](../../../../characteristic-polynomial.md) is $\chi_A(t)=t^n$. The [Cayley-Hamilton theorem](../../../../cayley-hamilton-theorem-split.md) then gives $A^n=0$. Hence

$$
\boxed{A^n=0\quad\Longleftrightarrow\quad\operatorname{spec}(A)=\{0\}.}
$$

This is the criterion for a [nilpotent matrix](../../../../nilpotent-matrix.md).

**Symmetric case.** Here a [symmetric matrix](../../../../symmetric-matrix.md) is understood to be real. The [spectral theorem](../../../../spectral-theorem.md) gives $A=QDQ^T$ with $Q$ orthogonal and $D$ real diagonal. The previous result makes every diagonal entry zero, so $A=0$. Alternatively, choose $2^r\geq n$, so $A^{2^r}=0$. For every real [vector](../../../../vector.md) $x$,

$$
x^TA^{2^r}x=\left\|A^{2^{r-1}}x\right\|^2=0.
$$

It follows that $A^{2^{r-1}}=0$. Repeat until $A=0$. This uses positivity of the [quadratic form](../../../../quadratic-form-split.md) $x^TM^TMx$. The restriction to real symmetric, or complex [Hermitian matrices](../../../../hermitian-operator.md), matters: a complex matrix satisfying only $A^T=A$ need not have this positivity.

**The parameters and powers.** The first two columns of $T$ coincide, so $\det T=0$ for all $\alpha,\beta$. The sum of its principal two-by-two determinants, each a [minor of a matrix](../../../../minor-linear-algebra.md), is

$$
0+(\beta-1)+(\beta-\alpha)=2\beta-\alpha-1.
$$

Together with $\operatorname{tr}T=2+\beta$, this gives

$$
\chi_T(t)=t^3-(2+\beta)t^2+(2\beta-\alpha-1)t.
$$

For every [eigenvalue](../../../../eigenvalue.md) to vanish both remaining coefficients must be zero. Therefore

$$
\boxed{\beta=-2,\qquad\alpha=-5.}
$$

Direct multiplication at these values gives

$$
T=\begin{pmatrix}1&1&1\\1&1&-5\\1&1&-2\end{pmatrix},\qquad
T^2=\begin{pmatrix}3&3&-6\\-3&-3&6\\0&0&0\end{pmatrix},\qquad\boxed{T^3=0.}
$$

Indeed the first row of $T^2$ multiplied by $T$ is $3\operatorname{row}_1(T)+3\operatorname{row}_2(T)-6\operatorname{row}_3(T)=0$, and the second row is its negative.

**Geometry of repeated application.** For any parameters the [image of a linear map](../../../../image-of-a-linear-map.md) lies in the [span](../../../../linear-span.md) of $a=(1,1,1)^T$ and $b=(1,\alpha,\beta)^T$, since $Tx=(x_1+x_2)a+x_3b$. Thus it lies in a fixed [plane](../../../../plane.md) through the origin, independently of the input. When $a,b$ are independent its normal is $a\times b=(\beta-\alpha,1-\beta,\alpha-1)$; if they coincide, the image is a line and is still contained in a plane.

For $\alpha=-5,\beta=-2$, put $s=x_1+x_2$ and $t=x_3$. Then

$$
Tx=(s+t,s-5t,s-2t)^T,\qquad x'_1+x'_2-2x'_3=0.
$$

The columns span this entire [plane](../../../../plane.md), so $T$ has [rank](../../../../rank-one-quadratic-form.md) two. The next two steps are

$$
\boxed{T^2x=3(x_1+x_2-2x_3)(1,-1,0)^T,\qquad T^3x=0.}
$$

Thus the [image of a linear map](../../../../image-of-a-linear-map.md) contracts from a plane to a line and then to the origin under successive applications. The line from $T^2$ is precisely the [kernel](../../../../kernel-of-a-linear-map-split.md) of $T$.

## ↑ Ancestors (12)

1. [4](../4.md)
2. [Paper 1](../../paper-1-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
