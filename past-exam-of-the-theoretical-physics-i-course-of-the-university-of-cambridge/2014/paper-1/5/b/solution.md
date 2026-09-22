<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

First fix the source at the spatial origin. [Fourier transform](../../../../../fourier-transform-split.md) replaces $\partial_t$ by $-i\omega$ and $\nabla$ by $i\mathbf k$ in the free term. Multiplication by a static background becomes a [momentum](../../../../../momentum-split.md) convolution; the [derivative](../../../../../derivative.md) in $A\cdot\partial G$ acts on the [Green function](../../../../../green-s-function-split.md), so it carries the internal [momentum](../../../../../momentum-split.md) $\mathbf k'$. Consequently

$$
\boxed{(k^2+m^2-\omega^2)G(\mathbf k;\omega)
+2e\int\frac{d^3k'}{(2\pi)^3}
[\omega A^0(\mathbf k-\mathbf k')-\mathbf A(\mathbf k-\mathbf k')\cdot\mathbf k']
G(\mathbf k';\omega)=1.}
$$

The transformed point source supplies the right-hand side one. The signs follow from $A^\mu\partial_\mu=A^0\partial_t+\mathbf A\cdot\nabla$ in these conventions.

**Source-position qualification.** For a nonuniform $A(\mathbf r)$, the general [Green function](../../../../../green-s-function-split.md) is not [translation](../../../../../translation-geometry.md) invariant. In the printed basis $e^{i\mathbf k\cdot(\mathbf r-\mathbf r')}$, its coefficient must also depend on $\mathbf r'$, and the convolution contains an extra factor $e^{i(\mathbf k-\mathbf k')\cdot\mathbf r'}$. The displayed source equation is valid for $\mathbf r'=0$, or with the background itself expressed in coordinates centred on that source. Equivalently, a general spatial Fourier [Green function](../../../../../green-s-function-split.md) has two [momentum](../../../../../momentum-split.md) arguments and a momentum-delta-function source. Staticity alone permits the time-difference transform, not a general position-difference-only transform.

## ↑ Ancestors (15)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2014](../../../split.md)
5. [Past exam of the theoretical physics I course of the University of Cambridge](../../../../split.md)
6. [Theoretical Physics I course of the University of Cambridge](../../../../../theoretical-physics-i-course-of-the-university-of-cambridge.md)
7. [Theoretical Physics course of the University of Cambridge](../../../../../theoretical-physics-course-of-the-university-of-cambridge.md)
8. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
11. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
12. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
13. [University of Cambridge](../../../../../university-of-cambridge-split.md)
14. [List of universities](../../../../../list-of-universities.md)
15. [Codex Wiki](../../../../../split.md)
