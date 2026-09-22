<h1 id="s01/2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

On the upper semicircular [contour](../../../../../complex-integration-contour.md), $|z|=R$ and the [reverse triangle inequality](../../../../../reverse-triangle-inequality.md) gives $|z^4+1|\ge R^4-1>0$. Its [arc length](../../../../../arc-length.md) is $\pi R$, so the [estimation lemma](../../../../../estimation-lemma.md) gives

$$
\boxed{\left|\int_{\gamma_R}\frac{z^2}{z^4+1}\,dz\right|\le\frac{\pi R^3}{R^4-1}\longrightarrow0.}
$$

The arc is open, so an ordinary integral sign is appropriate even though the source uses a closed-integral symbol there. Subtracting the vanishing arc contribution from the closed [contour integral](../../../../../contour-integral.md) gives the real-line [improper integral](../../../../../improper-integral.md) $\pi/\sqrt2$. Its integrand is an [even function](../../../../../even-function.md), and its tail is $O(x^{-2})$, ensuring convergence. Thus

$$
\boxed{\int_0^\infty\frac{x^2}{x^4+1}\,dx=\frac{\pi}{2\sqrt2}.}
$$

## ↑ Ancestors (13)

1. [C](../c.md)
2. [2](../../2.md)
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
