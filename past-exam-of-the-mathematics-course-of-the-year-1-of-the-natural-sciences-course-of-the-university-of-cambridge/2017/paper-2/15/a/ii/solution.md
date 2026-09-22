<h1 id="15/a/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Use $u=\cos x$, so $du=-\sin x\,dx$. Up to an overall minus sign, the differential form becomes

$$
(2y+3y^4u)\,du+(u+4y^3u^2)\,dy=0.
$$

Seeking a [monomial integrating factor](../../../../../../monomial-integrating-factor.md) $u^\alpha y^\beta$, equality of mixed [derivatives](../../../../../../derivative.md) gives

$$
2(\beta+1)=\alpha+1,\qquad3(\beta+4)=4(\alpha+2).
$$

These give $\alpha=1,\beta=0$, so the [integrating factor](../../../../../../integrating-factor.md) in the original variables is

$$
\boxed{\mu(x)=\cos x}.
$$

One may verify exactness directly without relying on invertibility of the [cosine](../../../../../../cosine.md) substitution:

$$
\cos x\,[M\,dx+N\,dy]
=-d\left(y\cos^2x+y^4\cos^3x\right).
$$

Thus the implicit [first integral](../../../../../../first-integral.md) is

$$
\boxed{y\cos^2x+y^4\cos^3x=C}.
$$

The equivalence with the [differential equation](../../../../../../differential-equation-split.md) holds directly where $\cos x\ne0$. The zero solution $y=0$ is included at $C=0$. At a zero of $\cos x$, the original graph equation requires $y=0$ for any finite [differentiable](../../../../../../differentiable-function.md) continuation, so no extra finite graph with nonzero $y$ is created by multiplying by the vanishing factor. If one allows vertical parametrized integral curves of the differential form, $x=\pi/2+n\pi$ is also such a curve and is already contained in the level set $C=0$.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [A](../../a.md)
3. [15](../../../15.md)
4. [Paper 2](../../../../paper-2-split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the year 1 of the natural sciences course of the University of Cambridge](../../../../../../mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
