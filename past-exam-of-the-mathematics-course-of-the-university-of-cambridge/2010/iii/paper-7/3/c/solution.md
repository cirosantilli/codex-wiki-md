<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Products below combine [matrix multiplication](../../../../../../matrix-multiplication.md) with the [wedge product of differential forms](../../../../../../wedge-product-of-differential-forms.md) of [differential forms](../../../../../../differential-form-split.md). Differentiate the [projection](../../../../../../projection-linear-algebra.md) identity $p^2=p$ to get

$$
(dp)p+p\,dp=dp,\qquad\boxed{p\,dp=dp(1-p)}.
$$

Multiplying by $p$ on both sides also gives $p\,dp\,p=0$; applying the same argument to $1-p$ gives $(1-p)dp(1-p)=0$. Thus at each point $dp$ is off-diagonal relative to $\operatorname{im}p\oplus\ker p$, whereas $(dp)^2$ is diagonal and commutes with $p$. For $\omega=p(dp)^2$,

$$
\omega^k=p(dp)^{2k}\quad(k\geq1),\qquad d\omega=(dp)^3,
$$

because $d(dp)=0$.

The [graded Leibniz rule](../../../../../../graded-leibniz-rule.md) and cyclicity of the [matrix trace](../../../../../../matrix-trace.md) give, since $\omega$ has even degree,

$$
d\operatorname{tr}(\omega^k)=k\operatorname{tr}\bigl((d\omega)\omega^{k-1}\bigr).
$$

Here $(d\omega)\omega^{k-1}$ is off-diagonal: $(dp)^3$ is off-diagonal and every power of $\omega$ is diagonal. Its [matrix trace](../../../../../../matrix-trace.md) is zero. Hence $\boxed{d\operatorname{tr}(\omega^k)=0}$ for every $k\geq1$; for $k=0$ the trace is the constant matrix size.

For the [determinant](../../../../../../determinant.md), work over the commutative algebra of even [differential forms](../../../../../../differential-form-split.md). If $f(0)=1$, write $f(\omega)=I+N$, where $N$ has strictly positive degree and is nilpotent for dimensional reasons. The finite [power series](../../../../../../power-series.md) identity

$$
\det f(\omega)=\exp\bigl(\operatorname{tr}\log(I+N)\bigr),\qquad
\log(I+N)=\sum_{j\geq1}\frac{(-1)^{j+1}}jN^j
$$

holds over this algebra, as follows either from the formal determinant identity over characteristic-zero commutative rings or by differentiating $\det(I+sN)$ in the scalar variable $s$. Each $N^j$ is a linear combination of positive powers of $\omega$. The [matrix trace](../../../../../../matrix-trace.md) of the logarithm is therefore a [closed differential form](../../../../../../closed-differential-form.md), and its finite exponential is closed by the [graded Leibniz rule](../../../../../../graded-leibniz-rule.md). Thus $\boxed{d\det f(\omega)=0}$. The [projection connection](../../../../../../projection-connection.md) interprets $\omega$ as the curvature of $p\,d$ on $\operatorname{im}p$, but the proof above directly establishes both closedness claims.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 7](../../../paper-7-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
