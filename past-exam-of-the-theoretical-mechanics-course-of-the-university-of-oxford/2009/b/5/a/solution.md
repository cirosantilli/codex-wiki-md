<h1 id="b/5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Split $I$ into the two tails and the interval $|k-k_*|<\delta$. On each tail $\psi'$ has a fixed nonzero sign, so changing variable to $s=\psi(k)$ produces a nonstationary Fourier integral. Under the usual decay and regularity needed for [integration by parts](../../../../../integration-by-parts.md), these pieces are $O(t^{-1})$.

Near the nondegenerate stationary point, make the signed local change

$$
z=\operatorname{sgn}(k-k_*)\sqrt{2[\psi(k)-\psi(k_*)]/\psi''(k_*)}.
$$

It has $dk/dz=1$ at zero and makes the phase exactly $\psi(k_*)+\psi''(k_*)z^2/2$. The transformed amplitude tends to $f(k_*)$. Scale $z$ by $t^{-1/2}$ and use the [Fresnel integral](../../../../../fresnel-integral.md) to obtain

$$
\boxed{I(t)=f(k_*)e^{it\psi(k_*)+i\pi/4}\sqrt{\frac{2\pi}{t\psi''(k_*)}}+o(t^{-1/2}).}
$$

The $O(t^{-1})$ tails are smaller than this leading stationary contribution. If $\psi''(k_*)<0$, complex conjugation of the Gaussian phase changes the phase correction to $-\pi/4$ and replaces the second derivative by its absolute value:

$$
\boxed{I(t)=f(k_*)e^{it\psi(k_*)-i\pi/4}\sqrt{\frac{2\pi}{t|\psi''(k_*)|}}+o(t^{-1/2}).}
$$

When the leading coefficient is nonzero this may be written as an [asymptotic equivalence](../../../../../asymptotic-equivalence.md). For full rigor, continuity of an arbitrary amplitude alone is not sufficient for the stated nonstationary $O(t^{-1})$ rate, nor does it ensure convergence of an infinite integral. Piecewise differentiability with integrable derivative, bounded variation, or an equivalent localization/decay hypothesis supplies the usual missing assumption. The exponentially decaying beam amplitude below has the required piecewise regularity.

## ↑ Ancestors (13)

1. [A](../a.md)
2. [5](../../5.md)
3. [B](../../../b.md)
4. [2009](../../../../2009-split.md)
5. [Past exam of the theoretical mechanics course of the University of Oxford](../../../../split.md)
6. [Theoretical mechanics course of the University of Oxford](../../../../../theoretical-mechanics-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
