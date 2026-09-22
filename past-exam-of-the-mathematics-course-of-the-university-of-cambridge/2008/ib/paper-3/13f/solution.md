<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

Let $p=(x_0,y_0)$, $a=f_x(p)$ and $b=f_y(p)$. For sufficiently small $h,k$, decompose the increment into an $x$-segment at height $y_0+k$ and a $y$-segment at $x_0$. The one-variable [mean value theorem](../../../../../mean-value-theorem.md) applies on each segment because existence of its partial derivative gives continuity along the segment. Thus, when both increments are nonzero,

$$
f(x_0+h,y_0+k)-f(p)=h f_x(x_0+\theta h,y_0+k)+k f_y(x_0,y_0+\eta k)
$$

for some $0<\theta,\eta<1$. The same formula with the absent segment omitted covers zero increments. Continuity of both [partial derivatives](../../../../../partial-derivative.md) at $p$ makes the remainder after subtracting $ah+bk$ at most $\varepsilon(|h|+|k|)$ for small increments, and hence at most $\sqrt2\varepsilon\sqrt{h^2+k^2}$. Therefore **the [Fréchet derivative](../../../../../frechet-derivative.md) is $(h,k)\mapsto ah+bk$**. Continuity throughout the disc is not required; continuity at the point suffices.

For the [determinant](../../../../../determinant.md), expand by [multilinearity of the determinant](../../../../../multilinearity-of-the-determinant.md) in the columns of $I+H$. Taking no perturbed column gives one; taking exactly one gives $\operatorname{tr}H$; all other terms have degree at least two in the entries of $H$. Since matrix-entry functionals are bounded in any finite-dimensional norm, their sum is $O(\|H\|^2)$. Hence

$$
\det(I+H)=1+\operatorname{tr}H+O(\|H\|^2),\qquad\boxed{D\det_I(H)=\operatorname{tr}H.}
$$

For invertible $A$, [multiplicativity of the determinant](../../../../../multiplicativity-of-the-determinant.md) gives $\det(A+H)=\det A\det(I+A^{-1}H)$. The bounded linear map $H\mapsto A^{-1}H$ transfers the preceding remainder estimate, giving the [derivative of the determinant](../../../../../derivative-of-the-determinant.md)

$$
\boxed{D\det_A(H)=\det A\operatorname{tr}(A^{-1}H).}
$$

To justify an open invertible neighborhood, let $\|K\|<1$. Completeness and submultiplicativity make the [Neumann series](../../../../../neumann-series.md) $S=\sum_{j=0}^\infty(-K)^j$ converge in matrix norm. Multiplying finite partial sums by $I+K$ gives $I-(-K)^{N+1}$, which tends to $I$. Continuity of multiplication proves $(I+K)S=S(I+K)=I$. Thus **$I+K$ is invertible**, and the series gives $(I+H)^{-1}=I-H+O(\|H\|^2)$ near zero.

Apply the first-derivative formula at $I+H$ to a test matrix $K$:

$$
\begin{aligned}
D\det_{I+H}(K)&=[1+\operatorname{tr}H+O(\|H\|^2)]\operatorname{tr}[(I-H+O(\|H\|^2))K]\\
&=\operatorname{tr}K+\operatorname{tr}H\operatorname{tr}K-\operatorname{tr}(HK)+O(\|H\|^2\|K\|).
\end{aligned}
$$

The last estimate is uniform for $\|K\|\le1$, so it proves differentiability of the derivative in the operator norm, rather than merely a directional second derivative. The [second derivative of the determinant](../../../../../second-derivative-of-the-determinant.md) is the symmetric [bilinear map](../../../../../bilinear-map.md)

$$
\boxed{D^2\det_I(H,K)=\operatorname{tr}H\operatorname{tr}K-\operatorname{tr}(HK).}
$$

Its symmetry follows from $\operatorname{tr}(HK)=\operatorname{tr}(KH)$.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
