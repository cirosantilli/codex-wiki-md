<h1 id="14a/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The mean of $f$ is zero. Its [Fourier cosine series](../../../../../../../fourier-cosine-series.md) coefficients are

$$
\begin{aligned}
A_n
&=\frac1\pi\left[
\int_0^\pi\left(\frac\pi2-\theta\right)\cos(n\theta)\,d\theta
+\int_\pi^{2\pi}\left(\theta-\frac{3\pi}2\right)\cos(n\theta)\,d\theta
\right]\\
&=\frac{2(1-(-1)^n)}{\pi n^2}.
\end{aligned}
$$

Thus $A_n=0$ for [even](../../../../../../../even-function.md) $n$ and $A_n=4/(\pi n^2)$ for [odd](../../../../../../../odd-function.md) $n$. Substitution into part (i) yields

$$
\boxed{
\phi(r,\theta)
=\log r-1
+\frac4\pi
\sum_{\substack{n\geq1\\ n\ {\rm odd}}}
\frac{\cosh(n(\log r-1))}{n^2\cosh n}\cos(n\theta)
}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [14A](../../../14a.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [Ib](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
