<h1 id="12/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $D=1+\omega^2$, with $\omega>0$. A particular solution of the [forced harmonic oscillator](../../../../../forced-harmonic-oscillator.md) is $y_p=e^{-t}(at+b)$. Substitution gives $Da=2$ and $Db-2a=0$, hence $a=2/D$ and $b=4/D^2$. Adding $A\cos\omega t+B\sin\omega t$ and imposing the two initial conditions gives $A=-4/D^2$ and $B=2(1-\omega^2)/(\omega D^2)$. Thus

$$
y(t)=e^{-t}\left(\frac{2t}{D}+\frac4{D^2}\right)-\frac4{D^2}\cos\omega t+\frac{2(1-\omega^2)}{\omega D^2}\sin\omega t.
$$

The first term tends to zero. The amplitude of the surviving sinusoid is

$$
\boxed{\sqrt{A^2+B^2}=\frac{2}{\omega(1+\omega^2)}.}
$$

As an independent interpretation, the [residual amplitude of an oscillator after an integrable force](../../../../../residual-amplitude-of-an-oscillator-after-an-integrable-force.md) is $\omega^{-1}|\int_0^\infty F(t)e^{-i\omega t}dt|$. Here that integral is $2/(1+i\omega)^2$, giving the same result.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [12](../../12.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
