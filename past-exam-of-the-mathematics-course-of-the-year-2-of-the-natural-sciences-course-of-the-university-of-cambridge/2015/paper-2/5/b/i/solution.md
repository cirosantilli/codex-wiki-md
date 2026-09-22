<h1 id="5/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Substitution gives

$$
\widetilde y(\omega)=\frac{-i}{(\omega-2i)(\omega-i-2)(\omega-i+2)}.
$$

The inverse [Fourier transform](../../../../../../fourier-transform-split.md) is $(2\pi)^{-1}\int_{\mathbb R}\widetilde y(\omega)e^{i\omega t}d\omega$. For $t<0$, close clockwise in the lower half-plane, where there are no poles; hence $y(t)=0$.

For $t>0$, close counterclockwise in the upper half-plane. The three simple-pole [residues](../../../../../../residue.md) of the full inversion integrand are

$$
\begin{array}{c|c}
\omega&\operatorname{Res}(\widetilde y e^{i\omega t})\\\hline
2i&ie^{-2t}/5\\
2+i&(1-2i)e^{(-1+2i)t}/20\\
-2+i&(-1-2i)e^{(-1-2i)t}/20
\end{array}.
$$

Multiplying their sum by $i$ and combining the conjugate exponential contributions yields

$$
\boxed{y(t)=\begin{cases}0,&t\leq0,\\[2pt]\dfrac1{10}\left[e^{-t}(2\cos2t-\sin2t)-2e^{-2t}\right],&t>0.\end{cases}}
$$

The large arcs vanish because the rational factor is $O(\omega^{-3})$ and the exponential is bounded on the chosen half-plane. At zero, the right-hand value and first derivative are both zero, matching the negative-time branch, so no unwanted delta or delta derivative appears in the second-order equation.

For an independent dynamical check, this is the [exponential forcing of an underdamped oscillator](../../../../../../exponential-forcing-of-an-underdamped-oscillator.md) with damping $\gamma=1$, natural frequency $\sqrt5$, damped frequency $2$, exponent $\beta=2$ and force amplitude $-1$. For positive time its substitution gives $y''+2y'+5y=-e^{-2t}$.

## ↑ Ancestors (14)

1. [I](../i.md)
2. [B](../../b.md)
3. [5](../../../5.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
