<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The input is even, so its [Fourier transform](../../../../../fourier-transform-split.md) is real and even. Decomposing the cosine into [complex exponentials](../../../../../complex-exponential-function.md) and integrating over its support gives

$$
\widetilde f(k)=\frac{\sin[(k-1)a]}{k-1}+\frac{\sin[(k+1)a]}{k+1}.
$$

Combining the fractions and using the angle addition formula yields

$$
\boxed{\widetilde f(k)=\frac{2k\cos a\sin(ak)-2\sin a\cos(ak)}{k^2-1},\qquad\lambda=2,\quad\mu=-2.}
$$

The apparent [poles](../../../../../pole.md) at $k=\pm1$ are [removable singularities](../../../../../removable-singularity.md); either the integral or the sine-quotient limit gives $\widetilde f(\pm1)=a+\sin(2a)/2$.

If $\cos a\ne0$, expansion of the denominator gives

$$
\widetilde f(k)=\frac{2\cos a\sin(ak)}k-\frac{2\sin a\cos(ak)}{k^2}+O(|k|^{-3}).
$$

The oscillatory envelope is therefore $O(|k|^{-1})$. At $a=\pi/2+n\pi$, $n=0,1,2,\ldots$, the endpoint values vanish and the first term cancels:

$$
\boxed{\cos a=0:\quad\widetilde f(k)=-\frac{2\sin a\cos(ak)}{k^2}+O(|k|^{-4}).}
$$

This gives an $O(|k|^{-2})$ envelope. At general $a$ the truncation creates jumps in the function; at these special values it leaves the function continuous but creates jumps in its first [derivative](../../../../../derivative.md). Each additional degree of endpoint smoothness gives another inverse power, as explained by [Fourier decay from a derivative jump](../../../../../fourier-decay-from-a-derivative-jump.md). The exact example is the [Fourier transform of a truncated cosine](../../../../../fourier-transform-of-a-truncated-cosine.md); isolated zeros of its oscillatory factors do not change the envelope order.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
