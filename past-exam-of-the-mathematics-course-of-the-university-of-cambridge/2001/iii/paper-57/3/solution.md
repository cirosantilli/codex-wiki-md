<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Insert a smooth exact solution, so $f(y(t))=y'(t)$ and $g(y(t))=y''(t)$. Expand about $t_n$. The residual, left side minus right side, has the formal differential-operator symbol

$$
\mathcal R(z)=e^z-e^{-z}-\frac7{15}z(e^z+e^{-z})-\frac{16}{15}z+\frac1{15}z^2(e^z-e^{-z}),\qquad z=hD.
$$

Its odd symmetry makes every even coefficient vanish. The coefficients of $z,z^3,z^5$ are respectively

$$
2-\frac{14}{15}-\frac{16}{15}=0,\qquad
\frac13-\frac7{15}+\frac2{15}=0,\qquad
\frac1{60}-\frac7{180}+\frac1{45}=0.
$$

The next coefficient is $1/4725\ne0$, giving

$$
\mathcal R(hD)y(t_n)=\frac{h^7}{4725}y^{(7)}(t_n)+O(h^9).
$$

Hence the [local truncation error](../../../../../local-truncation-error.md) has exact defect order seven and **the method has order six**. The zero-step [characteristic polynomial](../../../../../characteristic-polynomial.md) is $\zeta^2-1$, whose two unit roots are simple, so it is also [zero-stable](../../../../../zero-stability.md). With sufficiently accurate starting values and exact $g=f'f$ evaluations, the usual accumulation of defects gives sixth-order [global error](../../../../../global-discretization-error.md). This is the [symmetric sixth-order two-derivative method](../../../../../symmetric-sixth-order-two-derivative-method.md); approximate evaluations of $g$ must preserve the required accuracy if that order is to be retained.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 57](../../paper-57-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
