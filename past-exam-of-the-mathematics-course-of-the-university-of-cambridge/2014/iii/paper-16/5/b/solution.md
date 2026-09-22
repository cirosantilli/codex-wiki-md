<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Use the normalization in which a projective line has area $2\pi$. On the affine chart of [Complex projective space](../../../../../../complex-projective-space.md) where $Z_0\ne0$, set $w_j=Z_j/Z_0$ and $S=1+\sum_j|w_j|^2$. Define the [Fubini-Study form](../../../../../../fubini-study-form.md) by

$$
\boxed{\omega_{\mathrm{FS}}=i\partial\bar\partial\log S
=i\sum_{j,k}\frac{S\delta_{jk}-\bar w_jw_k}{S^2}\,dw_j\wedge d\bar w_k.}
$$

On another chart the corresponding potential differs by $\log|h|^2$ for a nowhere-zero [holomorphic function](../../../../../../holomorphic-function.md) $h$, whose $\partial\bar\partial$ is zero. Thus these local [differential forms](../../../../../../differential-form-split.md) glue to a global form. It is real and closed. Its Hermitian coefficient matrix is positive definite, since for $v\ne0$ the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\sum_{j,k}\frac{S\delta_{jk}-\bar w_jw_k}{S^2}v_j\bar v_k
=\frac{S|v|^2-|\sum_j\bar w_jv_j|^2}{S^2}\geq\frac{|v|^2}{S^2}>0.
$$

Hence it is a [Kähler form](../../../../../../kahler-form.md) and in particular a [symplectic form](../../../../../../symplectic-form.md).

On a [complex projective line](../../../../../../complex-projective-line.md) with $w=x+iy$ this is $2(1+|w|^2)^{-2}dx\wedge dy$, whose total area is $2\pi$. Thus $[\omega_{\mathrm{FS}}/(2\pi)]$ is the positive generator, equivalently $c_1(\mathcal O(1))$. Another common normalization uses half this form and gives line area $\pi$; the scale must be carried consistently into [symplectic reduction](../../../../../../symplectic-reduction.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
