<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\tau=T-t$ and set

$$
V(t,z)=\exp\{P(\tau)+Q(\tau)z+R(\tau)z^2\}.
$$

Then

$$
\frac{V_z}{V}=Q+2Rz,
\qquad
\frac{V_{zz}}V=2R+(Q+2Rz)^2,
\qquad
\frac{V_t}V=-(\dot P+\dot Qz+\dot Rz^2).
$$

For $B(z)=a-bz$ and $C(z)=c$, matching constant, linear, and quadratic coefficients gives

$$
\dot R
=2c^2R^2+2(\theta\rho c-b)R+\frac12\theta(\theta-1),
$$



$$
\dot Q
=2aR+(\theta\rho c-b)Q+2c^2QR,
$$

and

$$
\dot P=aQ+c^2R+\frac12c^2Q^2.
$$

The terminal condition becomes $P(0)=Q(0)=R(0)=0$. The first equation is a [Riccati equation](../../../../../../riccati-equation.md); once it is solved, the second is linear in $Q$, followed by direct integration for $P$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 211](../../../paper-211-split.md)
4. [Iii](../../../split.md)
5. [2022](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
