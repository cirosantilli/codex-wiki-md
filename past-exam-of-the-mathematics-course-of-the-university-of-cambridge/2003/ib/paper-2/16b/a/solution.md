<h1 id="16b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use $\widehat f(\lambda)=(2\pi)^{-1/2}\int_{\mathbb R}e^{-i\lambda x}f(x)\,dx$. The transform statement requires sufficient decay and regularity for the transform and its [derivatives](../../../../../../derivative.md); functions in the [Schwartz space](../../../../../../schwartz-space.md) suffice, and all the functions constructed below belong to that space. Integration by parts twice and differentiation under the integral give

$$
\widehat{f''}=-\lambda^2\widehat f,\qquad
\widehat{x^2f}=-\widehat f''.
$$

Transforming the differential equation therefore gives

$$
\boxed{\widehat f''(\lambda)-\lambda^2\widehat f(\lambda)=\mu\widehat f(\lambda).}
$$

The differential equation by itself does not ensure that an ordinary [Fourier transform](../../../../../../fourier-transform.md) exists: $f=e^{x^2/2}$ solves it with $\mu=1$ but grows too rapidly. Thus the usual transformability assumptions are implicit in this part.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [16B](../../16b.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ib](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
