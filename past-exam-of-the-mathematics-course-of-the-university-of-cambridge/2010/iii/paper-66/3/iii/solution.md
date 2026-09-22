<h1 id="3/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The [conservation of mass](../../../../../../mass-conservation.md) equation is $h_t+(uh)_x=0$. The flat region changes on time scale $L/U$, whereas a transition has advection time $\delta/U$. Hence $h_t=O(Uh_0/L)$, and its flux change across the transition is $O(Uh_0\delta/L)$, small compared with the entering flux $Uh_0$. To leading order the transition is quasisteady and

$$
\boxed{uh=q(t)=U(t)h_0(t).}
$$

Eliminate $u=q/h$ in the longitudinal equation. Then $hu_x=-q(\log h)_x$, so

$$
hh_{xxx}=\frac{8\mu q}{\gamma}(\log h)_{xx}.
$$

Use $\xi=(x-L)/\delta$, with $\delta=\sqrt{ah_0}$, and use a prime for differentiation with respect to $\xi$. This gives the third-order equation

$$
\boxed{hh'''=B(\log h)'',\qquad B=\frac{8\mu Uh_0\sqrt{ah_0}}\gamma.}
$$

Here $h$ remains a dimensional thickness; only the longitudinal coordinate is scaled.

Match at the inner end to $h\to h_0$, $h'\to0$, $h''\to0$. Since $(hh''-h'^2/2)'=hh'''$, the first integral is

$$
hh''-\frac12h'^2=B\frac{h'}h.
$$

Divide by $h^{3/2}$ to obtain $(h'/\sqrt h)'=Bh'/h^{5/2}$. Its second integral, using the flat-film limit to fix the constant, is

$$
\boxed{h^{-1/2}\frac{dh}{d\xi}
=\frac{2B}{3h_0^{3/2}}\left[1-\left(\frac{h_0}h\right)^{3/2}\right]
=\frac{16\mu U\sqrt a}{3\gamma}\left[1-\left(\frac{h_0}h\right)^{3/2}\right].}
$$

Let $A=16\mu U\sqrt a/(3\gamma)>0$. In the overlap $h\gg h_0$, the equation gives $h'\sim A\sqrt h$, hence $h''\sim A^2/2$. The curvature of each physical interface is $h_{xx}/2\sim A^2/(4ah_0)$. Matching to the outer bubble curvature $1/a$ therefore requires $A=2\sqrt{h_0}$ and fixes the numerical coefficient:

$$
\boxed{U=\frac{3\gamma}{8\mu}\sqrt{\frac{h_0}a}.}
$$

Finally the uniform-film evolution becomes $\dot h_0=-3\gamma h_0^{3/2}/(8\mu L\sqrt a)$. If $h_0(0)=h_i$ at the start of the drainage regime, its solution is

$$
\boxed{h_0(t)=\left[h_i^{-1/2}+\frac{3\gamma}{16\mu L\sqrt a}t\right]^{-2}.}
$$

Thus [capillary drainage of a film between two bubbles](../../../../../../capillary-drainage-of-a-film-between-two-bubbles.md) gives an algebraic $t^{-2}$ decrease, and the two bubbles do not touch in finite time in this ideal model. As $h_0$ decreases, $h_0/\delta$ and $\delta/L$ become still smaller, so the geometric scale separation improves. At molecular thicknesses, [disjoining pressure](../../../../../../disjoining-pressure.md) and changes in the assumed [stress-free boundary condition](../../../../../../stress-free-boundary-condition.md) can invalidate the clean continuum-sheet description; the algebraic law alone makes no claim about that physical endpoint.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [3](../../3.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
