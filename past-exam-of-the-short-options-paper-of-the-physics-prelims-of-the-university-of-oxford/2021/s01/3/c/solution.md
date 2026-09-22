<h1 id="s01/3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

For $x>0$, the upper and lower boundary values on the [branch cut](../../../../../branch-cut.md) are

$$
F(-x+i0)=-\frac{e^{-x-i\sqrt x}}x,\qquad F(-x-i0)=-\frac{e^{-x+i\sqrt x}}x.
$$

Write $x=A_R$ for the outer endpoint distance on the cut. The upper path runs from $x=A_R$ to $x=\epsilon$, while the lower path runs back from $\epsilon$ to $A_R$; in both cases $dz=-dx$. Therefore

$$
\int_{C_3}F\,dz=-\int_\epsilon^{A_R}\frac{e^{-x-i\sqrt x}}x\,dx,\qquad
\int_{C_5}F\,dz=\int_\epsilon^{A_R}\frac{e^{-x+i\sqrt x}}x\,dx,
$$

and

$$
\boxed{\int_{C_3}F\,dz+\int_{C_5}F\,dz=2i\int_\epsilon^{A_R}e^{-x}\frac{\sin\sqrt x}{x}\,dx.}
$$

The source's limits zero and infinity require $\epsilon\to0$ and $R\to\infty$; they are not an exact identity on a finite [contour](../../../../../complex-integration-contour.md). For a concrete counterexample take $\epsilon=1/4$ and $A_R=1$: the finite real integral is at most $\int_{1/4}^1x^{-1/2}\,dx=1$, whereas the full-range integral is $\pi\operatorname{erf}(1/2)\simeq1.6352$, as evaluated in the next part. Near zero the combined integrand is $O(x^{-1/2})$, so the combined [improper integral](../../../../../improper-integral.md) converges, although the individual cut integrals have logarithmic divergences. At infinity the factor $e^{-x}$ ensures convergence. Consequently

$$
\boxed{\lim_{R\to\infty,\,\epsilon\to0}\left(\int_{C_3}F\,dz+\int_{C_5}F\,dz\right)=2i\int_0^\infty e^{-x}\frac{\sin\sqrt x}{x}\,dx.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [3](../../3.md)
3. [S01](../../../s01.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the short options paper of the physics Prelims of the University of Oxford](../../../../split.md)
6. [Short options paper of the physics Prelims of the University of Oxford](../../../../../short-options-paper-of-the-physics-prelims-of-the-university-of-oxford.md)
7. [Year 1 of the physics course of the University of Oxford](../../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
8. [Physics course of the University of Oxford](../../../../../physics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
