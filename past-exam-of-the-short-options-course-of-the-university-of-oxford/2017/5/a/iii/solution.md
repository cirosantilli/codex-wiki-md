<h1 id="5/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

With this convention, the [Fourier inversion theorem](../../../../../fourier-inversion-theorem.md) states that if $f,\widehat f\in L^1(\mathbb R)$, then

$$
f(x)=\frac1{2\pi}\int_{\mathbb R}\widehat f(s)e^{isx}\,ds
$$

almost everywhere and at every continuity point of $f$. Apply this to the continuous function in part (ii):

$$
e^{-a|x|}=\frac a\pi\int_{\mathbb R}\frac{e^{isx}}{a^2+s^2}\,ds.
$$

The denominator is even. Replacing $x$ by $-t$ and renaming the integration variable gives

$$
\boxed{\mathcal F\!\left(\frac1{a^2+x^2}\right)(t)=\frac\pi a e^{-a|t|}.}
$$

Both integrable members of this transform pair satisfy the inversion hypotheses.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [5](../../../5.md)
4. [2017](../../../../2017-split.md)
5. [Past exam of the short options course of the University of Oxford](../../../../split.md)
6. [Short options course of the University of Oxford](../../../../../short-options-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
