<h1 id="analysis/5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $\omega=e^{2\pi i/3}$ and integrate $1/(1+z^3)$ around the positively oriented sector from argument [zero](../../../../../zero-of-a-function.md) to $2\pi/3$, with outer radius $R>1$. The single pole inside is $z_0=e^{i\pi/3}$, with [residue](../../../../../residue.md) $1/(3z_0^2)=1/(3\omega)$. The outward real radial segment contributes $I_R=\int_0^R dx/(1+x^3)$; the return radial segment contributes $-\omega I_R$ because $(\omega x)^3=x^3$.

On the circular arc, $|1+z^3|\geq R^3-1$, so its integral has modulus at most $(2\pi R/3)/(R^3-1)\to0$. Thus the [residue theorem](../../../../../residue-theorem.md) yields

$$
(1-\omega)I=\frac{2\pi i}{3\omega}.
$$

Since $\omega(1-\omega)=\omega-\omega^2=i\sqrt3$,

$$
\boxed{\int_0^\infty\frac{dx}{1+x^3}=\frac{2\pi}{3\sqrt3}.}
$$

The ordinary improper integral converges at both endpoints, so no principal-value interpretation is needed here.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Analysis](../../../analysis.md)
4. [2005](../../../../2005-split.md)
5. [Past exam of the algebra, analysis and differential equations II course of the University of Oxford](../../../../split.md)
6. [Algebra, analysis and differential equations II course of the University of Oxford](../../../../../algebra-analysis-and-differential-equations-ii-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
