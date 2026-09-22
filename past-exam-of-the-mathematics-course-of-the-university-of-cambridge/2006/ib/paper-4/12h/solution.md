<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

In the [Poincare disc model](../../../../../poincare-disk-model.md), [hyperbolic lines](../../../../../hyperbolic-line.md) are diameters and circular arcs meeting the boundary circle orthogonally. In the [upper half-plane model](../../../../../poincare-half-plane-model.md), they are vertical lines and semicircles with centres on the real axis. The metric is conformal, so hyperbolic perpendicularity agrees with Euclidean perpendicularity.

Use an [isometry](../../../../../isometry.md) of the [hyperbolic plane](../../../../../hyperbolic-plane.md) to send an arbitrary line to the positive imaginary axis. For $P=x+iy$ with $x\ne0$, a point on that axis is $Q=iv$ with $v>0$. The [hyperbolic distance](../../../../../hyperbolic-distance.md) formula gives

$$
\cosh\rho(P,iv)=1+\frac{x^2+(y-v)^2}{2yv}=\frac{x^2+y^2+v^2}{2yv}.
$$

Put $R=\sqrt{x^2+y^2}$. The last expression is $(v+R^2/v)/(2y)$, uniquely minimized at $v=R$, since $v+R^2/v\geq2R$ with equality only there. Hence the unique closest point is $Q_0=iR$. The semicircle $|z|=R$ passes through $P$ and $Q_0$ and meets the imaginary axis at a right angle. Conversely a semicircle centred at a real number $b$ can meet that axis orthogonally only if $b=0$; a vertical line cannot furnish such a crossing. Thus the perpendicular is unique. Isometries transfer both uniqueness and minimization back to the original line.

For $P$ on the specified second semicircle, $a-r\leq x\leq a+r$ and $R=|P|\leq a+r$. Its perpendicular to the axis is the semicircle just found, with radius $R$. Moreover

$$
\cosh d(P,L_1)=\frac{R}{y},\qquad \tanh d(P,L_1)=\frac{x}{R}.
$$

Since $t\leq\operatorname{artanh}t$ for $0\leq t<1$, we obtain

$$
\boxed{d(P,L_1)\geq\frac{x}{R}\geq\frac{a-r}{a+r}>0.}
$$

This is uniform over the whole semicircle, including points arbitrarily close to the ideal endpoints.

Finally send any first line of an ultraparallel pair to the axis by an [isometry](../../../../../isometry.md) of the [hyperbolic plane](../../../../../hyperbolic-plane.md). The second cannot be a vertical line, since that would share the ideal point at infinity. Its two finite endpoints lie on the same side of zero; otherwise its semicircle would meet the axis, or share the endpoint zero. Reflect horizontally if necessary, so those endpoints are $a-r,a+r$ with $a>r>0$. The uniform estimate above then gives

$$
\boxed{d(L_1,L_2)\geq\frac{a-r}{a+r}>0.}
$$

Thus [ultraparallel hyperbolic lines](../../../../../ultraparallel-hyperbolic-lines.md) have strictly positive separation; disjointness in the interior alone would not suffice.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
