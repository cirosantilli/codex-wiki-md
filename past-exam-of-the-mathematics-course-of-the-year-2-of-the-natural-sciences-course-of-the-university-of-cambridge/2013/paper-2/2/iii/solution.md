<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Put $x=\sqrt{s}R>0$. Orthogonality of the [Legendre polynomials](../../../../../legendre-polynomial.md) lets us match each degree separately. Continuity of the field and its radial derivative gives

$$
B_\ell j_\ell(x)=\frac{A_\ell}{R^{\ell+1}},\qquad \sqrt{s}B_\ell j_\ell'(x)=-\frac{(\ell+1)A_\ell}{R^{\ell+2}}.
$$

Eliminate $A_\ell$ by multiplying the first equation by $(\ell+1)/R$ and adding it to the second. A nonzero mode therefore requires

$$
\boxed{xj_\ell'(x)+(\ell+1)j_\ell(x)=0.}
$$

This argument avoids dividing by a potentially zero boundary value. Apply the supplied recurrence with $\nu=\ell-1$:

$$
xj_\ell'(x)+(\ell+1)j_\ell(x)=xj_{\ell-1}(x).
$$

Consequently [spherical Helmholtz matching to a decaying harmonic exterior](../../../../../spherical-helmholtz-matching-to-a-decaying-harmonic-exterior.md) gives

$$
\boxed{j_{\ell-1}(\sqrt{s}R)=0,}
$$

where $j_{-1}(x)=\cos x/x$ for the $\ell=0$ sector.

**The original PDF has an index error here:** it prints $f_\ell$ rather than $f_{\ell-1}$ in the resulting eigenvalue condition. This cannot be repaired by silently choosing another normalization. If $j_\ell(x)$ itself were zero at a positive matching root, the boundary equation would also give $j_\ell'(x)=0$, contradicting uniqueness for this nonzero solution of a regular differential equation at that point.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2013](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
