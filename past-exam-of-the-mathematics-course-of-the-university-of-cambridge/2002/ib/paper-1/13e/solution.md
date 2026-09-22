<h1 id="13e/solution">Solution</h1>

↑ **Parent:** [13E](../13e.md)

For $g(z)=(az+b)/(cz+d)$ with real coefficients and $ad-bc=1$, direct subtraction from its conjugate gives

$$
\operatorname{Im}g(z)=\frac{\operatorname{Im}z}{|cz+d|^2},\qquad g'(z)=\frac1{(cz+d)^2}.
$$

The imaginary part remains positive, and the inverse transformation has the same form, so $g$ is a bijection of the upper half-plane. Moreover

$$
\frac{|dg(z)|}{\operatorname{Im}g(z)}=\frac{|dz|}{\operatorname{Im}z}.
$$

Thus every path has the same hyperbolic length as its image. Taking the infimum over connecting paths, and using the inverse for the reverse inequality, proves **every $g\in\Gamma$ is an [isometry](../../../../../isometry.md)**.

Likewise

$$
g(z)-g(w)=\frac{z-w}{(cz+d)(cw+d)}.
$$

Its squared modulus and the two imaginary-part factors cancel in the quotient, proving

$$
\boxed{h(g(z),g(w))=h(z,w)}.
$$

We can normalize any ordered distinct pair to $(i,iy)$ with $y>1$. First send $z=x_0+iy_0$ to $i$ by $(\zeta-x_0)/y_0$, a real determinant-one [Möbius transformation](../../../../../mobius-transformation.md) after rescaling its representing matrix. The stabilizer transformations

$$
k_\tau(\zeta)=\frac{\cos\tau\,\zeta+\sin\tau}{-\sin\tau\,\zeta+\cos\tau}
$$

fix $i$. Under the Cayley map $C(\zeta)=(\zeta-i)/(\zeta+i)$, direct substitution gives $C(k_\tau\zeta)=e^{2i\tau}C(\zeta)$. Choose $\tau$ to rotate the second point's nonzero disc coordinate onto the positive real axis. Its inverse image is $iy$ with $y=(1+|C|)/(1-|C|)>1$.

The vertical path from $i$ to $iy$ has length $\log y$. Any other path has length at least $\int|dy|/y\geq|\int dy/y|=\log y$, so $\rho(i,iy)=\log y$. Consequently

$$
\cosh\rho(i,iy)=\frac{y+y^{-1}}2=1+\frac{(y-1)^2}{2y}=1+\frac12h(i,iy).
$$

Invariance of both quantities transfers this equality back to every pair; coincident points satisfy it as well. Therefore

$$
\boxed{\cosh\rho(z,w)=1+\frac{|z-w|^2}{2\operatorname{Im}z\operatorname{Im}w}}.
$$

For the right-triangle identity, normalize its right vertex to $i$ and one leg to the vertical [geodesic](../../../../../geodesic.md), with endpoint $iy$, $y>1$. The other leg lies on the unit semicircle, with endpoint $s+it$, $s^2+t^2=1$, $t>0$. These [geodesics](../../../../../geodesic.md) meet orthogonally at $i$, since the metric is conformal to the Euclidean metric. The semicircle is a [geodesic](../../../../../geodesic.md) because a real [Möbius transformation](../../../../../mobius-transformation.md) sends it to a vertical line; vertical lines are minimizing by the same length bound. The stabilizer [rotations](../../../../../rotation-mathematics.md) above can align any given tangent direction, giving this normal form for every right triangle.

If the legs have lengths $a,b$ and the opposite side has length $c$, the distance formula gives

$$
\cosh a=\frac{1+y^2}{2y},\qquad\cosh b=1+\frac{s^2+(t-1)^2}{2t}=\frac1t,
$$

and

$$
\cosh c=1+\frac{s^2+(t-y)^2}{2ty}=\frac{1+y^2}{2ty}.
$$

Thus the [hyperbolic Pythagorean theorem](../../../../../hyperbolic-pythagorean-theorem.md) is

$$
\boxed{\cosh a\cosh b=\cosh c}.
$$

## ↑ Ancestors (10)

1. [13E](../13e.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
