<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\tau>0$ be the first conjugate time and choose a nonzero [Jacobi field](../../../../../../jacobi-field.md) $J$ with $J(0)=J(\tau)=0$. It is normal by part 1(b), and $D_tJ(\tau)\ne0$, since zero value and derivative there would force $J=0$. Fix any $T>\tau$ and extend $J$ by zero to a continuous piecewise smooth [vector field](../../../../../../vector-field.md) $V$ on $[0,T]$.

For endpoint-vanishing fields, the [Riemannian index form](../../../../../../riemannian-index-form.md) is

$$
I(X,Y)=\int_0^T\bigl(\langle D_tX,D_tY\rangle-\langle R(X,\dot\gamma)\dot\gamma,Y\rangle\bigr)\,dt.
$$

Integration by parts on $[0,\tau]$ and the [Jacobi field](../../../../../../jacobi-field.md) equation give $I(V,V)=0$ and

$$
I(V,W)=\langle D_tJ(\tau),W(\tau)\rangle.
$$

Choose a smooth normal field $W$, zero at $0,T$, with $W(\tau)=-D_tJ(\tau)$. Then

$$
I(V+\varepsilon W,V+\varepsilon W)=-2\varepsilon|D_tJ(\tau)|^2+\varepsilon^2I(W,W)<0
$$

for sufficiently small positive $\varepsilon$. The corner in $V$ causes no difficulty: smooth endpoint-vanishing fields approximate $V+\varepsilon W$ in the [Sobolev space](../../../../../../sobolev-space-split.md) $H^1$, and the [Riemannian index form](../../../../../../riemannian-index-form.md) is continuous in this norm on the compact segment. A smooth approximant therefore still has negative index form.

Realize this smooth field as a fixed-endpoint curve variation using the [Riemannian exponential map](../../../../../../exponential-map-riemannian-geometry.md). The allowed [second variation of geodesic energy](../../../../../../second-variation-of-geodesic-energy.md) gives $E'(0)=0$ and $E''(0)<0$, so some nearby curve has energy less than $T/2$, the energy of the unit-speed reference [geodesic](../../../../../../geodesic.md). The [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) bounds its length by

$$
L^2\leq T\int_0^T|\dot c|^2\,dt=2TE<T^2.
$$

It is shorter than the reference segment. Thus **a geodesic cannot minimize beyond its first conjugate time**. This argument deliberately uses $T>\tau$; it does not rule out minimization up to the [conjugate point](../../../../../../conjugate-point.md) itself.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 16](../../../paper-16-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
