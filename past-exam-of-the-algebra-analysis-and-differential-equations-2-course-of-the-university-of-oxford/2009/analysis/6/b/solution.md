<h1 id="analysis/6/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a positively oriented simple closed piecewise smooth curve, a point $a$ inside it and a function $h$ [holomorphic](../../../../../holomorphic-function-split.md) on a neighborhood of the curve and its interior, Cauchy's differentiated integral formula is

$$
\boxed{h^{(m)}(a)=\frac{m!}{2\pi i}\int_\gamma\frac{h(z)}{(z-a)^{m+1}}dz\quad(m\ge0).}
$$

**The printed denominator uses $n+1$ while the [derivative](../../../../../derivative.md) and factorial use $m$.** The standard formula requires these indices to agree; the intended exponent in this display is $m+1$. The private transcription preserves the mismatch exactly.

For the following task, write $f(z)=zq(z)$ near zero with $q(0)=f'(0)\ne0$. Thus $H(z)=(z/f(z))^n=q(z)^{-n}$ extends holomorphically at zero, and is [holomorphic](../../../../../holomorphic-function-split.md) inside the specified contour because $f$ has no other zeros there. Now $f(z)^{-n}=H(z)/z^n$. Apply the correctly indexed formula with [derivative](../../../../../derivative.md) order $n-1$ to get

$$
\boxed{\int_\gamma\frac{dz}{f(z)^n}=\frac{2\pi i}{(n-1)!}\left[\frac{d^{n-1}}{dz^{n-1}}\left(\frac z{f(z)}\right)^n\right]_{z=0}.}
$$

Positive winding one supplies the orientation and multiplicity used in this expression.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [6](../../6.md)
3. [Analysis](../../../analysis.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
