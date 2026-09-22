<h1 id="2/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The intended [self-adjoint operator](../../../../../../self-adjoint-operator.md) identity is $\langle Lf,g\rangle=\langle f,Lg\rangle$, with the [inner product](../../../../../../inner-product.md) linear in its first argument. The printed second $Lf$ must be $Lg$. Taken literally, the printed identity forces $L=0$: put $g=0$ and then vary $g$. Its spectral conclusion is then trivial, but it does not define self-adjointness.

For the corrected identity, $\langle Lv,v\rangle$ is real. If $\operatorname{Im}\lambda\ne0$, the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) gives

$$
\|(L-\lambda I)v\|\|v\|\ge|\operatorname{Im}\langle(L-\lambda I)v,v\rangle|=|\operatorname{Im}\lambda|\|v\|^2.
$$

Thus $L-\lambda I$ is injective and bounded below, so its range is closed: a convergent image sequence has a [Cauchy sequence](../../../../../../cauchy-sequence.md) of preimages. Its range is dense because its [orthogonal complement](../../../../../../orthogonal-complement.md) is $\ker(L-\bar\lambda I)$, also zero by the same lower bound. Hence it is surjective with inverse norm at most $1/|\operatorname{Im}\lambda|$. Therefore

$$
\boxed{\Sigma(L)\subset\mathbb R.}
$$

## ↑ Ancestors (11)

1. [5](../5.md)
2. [2](../../2.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
