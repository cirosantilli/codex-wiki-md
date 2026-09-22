# Optimal aspect ratios of closed cylinders

↑ **Parent:** [Cylinder (geometry)](cylinder-geometry.md)

A closed [circular cylinder](circular-cylinder.md) of radius $a>0$ and length $\ell>0$ has [volume](volume.md) $\pi a^2\ell$ and total [surface area](surface-area.md) $2\pi a(a+\ell)$, including both end disks. At fixed area $A$, [Lagrange multipliers](lagrange-multiplier.md) for maximizing the volume give $\ell=2a$, hence

$$
a=\sqrt{\frac A{6\pi}},\qquad V_{\max}=\frac13\sqrt{\frac{A^3}{6\pi}}.
$$

Equivalently, eliminate $\ell=A/(2\pi a)-a$ and maximize $(A/2)a-\pi a^3$ on $0<a<\sqrt{A/(2\pi)}$. The derivative changes from positive to negative at the displayed radius, and the volume tends to zero at both ends.

For a cylinder inscribed in a [sphere](sphere.md) of radius $R$, the constraint is $a^2+\ell^2/4=R^2$. Maximizing $a^2+a\ell$ by [Lagrange multipliers](lagrange-multiplier.md) gives $\ell^2+2a\ell=4a^2$, so the positive aspect ratio is $\ell/a=\sqrt5-1$. It is independent of $R$. With $q=\ell/a$, the area is $2\pi R^2(1+q)/(1+q^2/4)$; differentiating this expression confirms the unique maximum on $q>0$.

## ↑ Ancestors (5)

1. [Cylinder (geometry)](cylinder-geometry.md)
2. [Geometry and topology](geometry-and-topology-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/19/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-year-1-of-the-natural-sciences-course-of-the-university-of-cambridge/2010/paper-2/19/b/solution.md)
