<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the standard [Fourier transform](../../../../../../../fourier-transform.md) on the whole real axis. The printed lower limit is missing a minus sign. For this integrable even function, its only obstruction to smoothness is the origin, so its high-frequency algebraic terms come from its local cusp:

$$
\frac1{1+|x|^3}=1-|x|^3+|x|^6-|x|^9+|x|^{12}-\cdots.
$$

Localize near zero with a smooth cutoff. The smooth polynomial terms, including $|x|^6=x^6$, contribute no algebraic cusp term; their localized transforms decay faster than any prescribed inverse power. The supplied half-line formula, interpreted away from $k=0$ in an Abel-regularized or [tempered distribution](../../../../../../../tempered-distribution.md) sense, gives the [Fourier transform of an algebraic cusp](../../../../../../../fourier-transform-of-an-algebraic-cusp.md)

$$
\mathcal F(|x|^p)(k)=\frac{2\Gamma(p+1)\cos[\pi(p+1)/2]}{|k|^{p+1}}\quad(k\ne0).
$$

For $p=3$ the cosine is $1$, and for $p=9$ it is $-1$. Both cusp coefficients in the local expansion are $-1$. Hence

$$
\boxed{\widehat f(k)=-\frac{12}{|k|^4}+\frac{2\,9!}{|k|^{10}}+O(|k|^{-16})}.
$$

The second coefficient is $2\,9!=725760$. The absence of a $|k|^{-7}$ term follows from the smooth even power $x^6$, not from neglecting an available correction.

One can verify the signs by [integration by parts](../../../../../../../integration-by-parts.md) on $2\operatorname{Re}\int_0^\infty e^{-ikx}(1+x^3)^{-1}dx$. Its endpoint derivatives first have nonzero relevant values $f^{(3)}(0)=-3!$ and $f^{(9)}(0)=-9!$, which contribute twice those values divided by $(ik)^4$ and $(ik)^{10}$. Higher derivatives are integrable on the half-line, justifying the displayed remainder after further integrations. Equivalently these coefficients are the [Fourier decay from a derivative jump](../../../../../../../fourier-decay-from-a-derivative-jump.md) at the origin.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 67](../../../../paper-67-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
