<h1 id="2/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The [distributional derivative](../../../../../distributional-derivative.md) is defined by $\langle u',\phi\rangle=-\langle u,\phi'\rangle$. Since [differentiation under the integral sign](../../../../../differentiation-under-the-integral-sign.md) gives $(\widehat\phi)'=\widehat{-i\xi\phi}$, we obtain

$$
\begin{aligned}
\langle\widehat{u'},\phi\rangle
&=\langle u',\widehat\phi\rangle
=-\langle u,(\widehat\phi)'\rangle
=\langle u,\widehat{i\xi\phi}\rangle\\
&=\langle\widehat u,i\xi\phi\rangle
=\langle i\xi\widehat u,\phi\rangle.
\end{aligned}
$$

This proves the [Fourier transform of a derivative](../../../../../fourier-transform-of-a-derivative.md) identity $\boxed{\widehat{u'}=i\xi\widehat u}$ for all [tempered distributions](../../../../../tempered-distribution.md).

If $u,u'\in H^s(\mathbb R)$, their [Fourier transforms](../../../../../fourier-transform-split.md) are represented by [locally square-integrable functions](../../../../../locally-square-integrable-function.md), and the identity identifies $\widehat{u'}$ with $i\xi\widehat u$ [almost everywhere](../../../../../almost-everywhere.md). Hence the [Sobolev norms](../../../../../sobolev-norm.md) satisfy

$$
\begin{aligned}
\|u\|_{H^{s+1}}^2
&=\int(1+\xi^2)^s(1+\xi^2)|\widehat u|^2\,d\xi\\
&=\int(1+\xi^2)^s|\widehat u|^2\,d\xi
+\int(1+\xi^2)^s|\widehat{u'}|^2\,d\xi,
\end{aligned}
$$

so $\boxed{u\in H^{s+1}(\mathbb R),\quad\|u\|_{H^{s+1}}^2=\|u\|_{H^s}^2+\|u'\|_{H^s}^2}$ for every real $s$.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [2](../../../2.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the fourier analysis course of the University of Oxford](../../../../split.md)
6. [Fourier analysis course of the University of Oxford](../../../../../fourier-analysis-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
