<h1 id="1/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For $0<\lambda<1$, the preceding change of variables and one [integration by parts](../../../../../../../integration-by-parts.md) give

$$
v(\lambda)
=-ie^{-i\lambda}-\lambda\int_\lambda^\infty\frac{e^{-ix}}x\,dx.
$$

Split the last [improper integral](../../../../../../../improper-integral.md) at one and add and subtract one on $(\lambda,1)$. Since $\int_\lambda^1dx/x=-\log\lambda$,

$$
\boxed{
v(\lambda)=\lambda\log|\lambda|-ie^{-i\lambda}
-\lambda\left[
\int_\lambda^1\frac{e^{-ix}-1}{x}\,dx
+\int_1^\infty\frac{e^{-ix}}x\,dx
\right]}.
$$

The definition also gives the [complex conjugate](../../../../../../../complex-conjugate.md) relation

$$
v(-\lambda)=-\overline{v(\lambda)}.
$$

Consequently, for $-1<\lambda<0$,

$$
\boxed{
v(\lambda)=\lambda\log|\lambda|-ie^{-i\lambda}
-\lambda\left[
\int_{|\lambda|}^1\frac{e^{ix}-1}{x}\,dx
+\int_1^\infty\frac{e^{ix}}x\,dx
\right]}.
$$

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [1](../../../1.md)
4. [Paper 327](../../../../paper-327-split.md)
5. [Iii](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
