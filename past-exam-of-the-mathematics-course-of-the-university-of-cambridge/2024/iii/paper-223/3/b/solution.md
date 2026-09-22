<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [Huber location estimator](../../../../../../huber-location-estimator.md) uses

$$
\psi_k(u)=\operatorname{clip}(u,-k,k),
\qquad
\psi_k'(u)=\mathbf1_{\{|u|<k\}}
$$

away from the two corners. At $F=N(\theta,1)$, symmetry gives $T(F)=\theta$, and for $Z\sim N(0,1)$,

$$
\mathbb E\psi_k'(Z)=\mathbb P(|Z|<k)=2\Phi(k)-1.
$$

Hence

$$
\operatorname{IF}(x;T,F)
=\frac{\operatorname{clip}(x-\theta,-k,k)}{2\Phi(k)-1},
$$

which is bounded in $x$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 223](../../../paper-223-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
