<h1 id="m/m4/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

For positive standard deviations $a,b$, substitute the two normal densities:

$$
f_V(v)=\frac1{\pi ab}\int_0^\infty u\exp\left[-\frac{u^2}{2}\left(a^{-2}+v^2b^{-2}\right)\right]du.
$$

The integral is $1/(a^{-2}+v^2b^{-2})$, by substituting the exponent's quadratic argument. Thus, with $c=b/a$,

$$
\boxed{f_V(v)=\frac{ab}{\pi(b^2+a^2v^2)}=\frac c{\pi(c^2+v^2)}.}
$$

This is a centered [Cauchy distribution](../../../../../../cauchy-distribution.md) of scale $c$. Since $P(X=0)=0$, the desired probability is

$$
\boxed{P(|Y|<|X|)=P(|V|<1)
=\frac2\pi\arctan\frac1c=\frac2\pi\arctan\frac ab.}
$$

## ↑ Ancestors (14)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [M4](../../../m4.md)
4. [M](../../../../m.md)
5. [2010](../../../../../2010-split.md)
6. [Past exam of the options II course of the University of Oxford](../../../../../split.md)
7. [Options II course of the University of Oxford](../../../../../../options-ii-course-of-the-university-of-oxford.md)
8. [Year 2 of the mathematics course of the University of Oxford](../../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
9. [Mathematics course of the University of Oxford](../../../../../../mathematics-course-of-the-university-of-oxford.md)
10. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
11. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
12. [University of Oxford](../../../../../../university-of-oxford-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
