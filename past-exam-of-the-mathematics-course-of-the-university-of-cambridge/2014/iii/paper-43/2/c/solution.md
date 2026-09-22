<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Introduce $y^\mu=x^\mu+i\theta\sigma^\mu\bar\theta$ and retain the same [Grassmann variables](../../../../../../grassmann-variable.md). The [supersymmetric derivatives in chiral coordinates](../../../../../../supersymmetric-derivatives-in-chiral-coordinates.md) follow from the [left Grassmann derivative](../../../../../../left-grassmann-derivative.md) chain rule. Differentiating $y$ gives

$$
\partial_\alpha y^\mu=i(\sigma^\mu\bar\theta)_\alpha,\qquad
\bar\partial_{\dot\alpha}y^\mu=-i(\theta\sigma^\mu)_{\dot\alpha}.
$$

The minus sign in the second relation comes from moving the odd [Grassmann derivative](../../../../../../grassmann-derivative.md) past $\theta$. Hence, as operators on a [superfield](../../../../../../superfield.md) expressed in $(y,\theta,\bar\theta)$,

$$
\left.\partial_\alpha\right|_x=\left.\partial_\alpha\right|_y+i(\sigma^\mu\bar\theta)_\alpha\partial_{y^\mu},\qquad
\left.\bar\partial_{\dot\alpha}\right|_x=\left.\bar\partial_{\dot\alpha}\right|_y-i(\theta\sigma^\mu)_{\dot\alpha}\partial_{y^\mu},
\qquad \partial_{x^\mu}=\partial_{y^\mu}.
$$

Substitution into the two [supersymmetric covariant derivatives](../../../../../../supersymmetric-covariant-derivative.md) adds the two unbarred spacetime terms and cancels the two barred ones:

$$
\boxed{D_\alpha=\left.\partial_\alpha\right|_y+2i(\sigma^\mu\bar\theta)_\alpha\partial_{y^\mu},\qquad
\bar D_{\dot\alpha}=-\left.\bar\partial_{\dot\alpha}\right|_y.}
$$

These operator equalities prove both requested actions on $V$. In particular, a [chiral superfield](../../../../../../chiral-superfield.md) becomes independent of $\bar\theta$ at fixed $y$. The TeX aid corrupts the second formula by replacing its ordinary barred derivative with a covariant one; the original PDF has the ordinary $-\bar\partial_{\dot\alpha}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
