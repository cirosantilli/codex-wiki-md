<h1 id="1/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The intended oscillatory factor is $e^{-ik\tau}$. Give the early-time endpoint the usual [i-epsilon prescription](../../../../../../feynman-i-epsilon-prescription.md) and set $x=-k\tau$. For an integer $p\geq0$,

$$
\begin{aligned}
I_p&=\int_{-\infty(1-i\epsilon)}^0e^{-ik\tau}(i\tau)^p\,d\tau\\
&=\frac{(-i)^p}{k^{p+1}}
\lim_{\epsilon\downarrow0}\int_0^\infty x^pe^{-(\epsilon-i)x}\,dx\\
&=\frac{(-i)^p\Gamma(p+1)}{k^{p+1}}
\lim_{\epsilon\downarrow0}(\epsilon-i)^{-(p+1)}
=\boxed{\frac{i\,p!}{k^{p+1}}}.
\end{aligned}
$$

It is therefore purely imaginary. Equivalently, rotating the contour to the negative imaginary $\tau$ axis turns the remaining integral into a real [Gamma integral](../../../../../../gamma-integral.md) and leaves one overall factor of $i$.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [1](../../1.md)
3. [Paper 312](../../../paper-312-split.md)
4. [Iii](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
