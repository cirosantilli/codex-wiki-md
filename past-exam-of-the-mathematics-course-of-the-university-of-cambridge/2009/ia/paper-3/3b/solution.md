<h1 id="3b/solution">Solution</h1>

↑ **Parent:** [3B](../3b.md)

A continuously differentiable [vector field](../../../../../vector-field.md) is an [irrotational vector field](../../../../../irrotational-vector-field.md) when its [curl](../../../../../curl.md) vanishes:

$$
\nabla\times\mathbf F=\mathbf0.
$$

For the global-potential construction, assume that the domain is connected and simply connected, or more generally that all closed-curve [line integrals](../../../../../line-integral.md) of $\mathbf F$ vanish. Then define the [potential of a conservative vector field](../../../../../potential-of-a-conservative-vector-field.md) by

$$
\boxed{V(\mathbf x)=-\int_{\mathbf x_0}^{\mathbf x}\mathbf F\cdot d\mathbf r.}
$$

Two paths with the same endpoints differ by a closed curve. On a [simply connected](../../../../../simply-connected-space.md) domain that curve can be spanned, or contracted through piecewise smooth spanning surfaces, inside the domain. [Stokes theorem](../../../../../stokes-theorem.md) gives zero circulation because the [curl](../../../../../curl.md) is zero. The value of $V$ is therefore path-independent and $V(\mathbf x_0)=0$. To compute a derivative, append a short coordinate segment to a path ending at $\mathbf x$. Then $V(\mathbf x+h\mathbf e_i)-V(\mathbf x)=-\int_0^hF_i(\mathbf x+s\mathbf e_i)\,ds$, so $\partial_iV=-F_i$.

The domain qualification is necessary and is implicit in the potential request. Curl-free alone on an arbitrary domain does not suffice: $\mathbf F=(-y,x,0)/(x^2+y^2)$ on the complement of the $z$-axis has zero [curl](../../../../../curl.md), but its circulation around a unit circle is $2\pi$. It has no single-valued global potential. The intended construction is valid on all of $\mathbb R^3$ for a smooth curl-free field, and on any other domain satisfying the condition above.

For the given spherical-coordinate field, the angular components have $rF_\theta=\cos\theta\cos\phi$ and $rF_\phi=m\sin\phi$, independent of $r$, so the $\theta$ and $\phi$ [curl](../../../../../curl.md) components vanish. The radial component is

$$
(\nabla\times\mathbf F)_r
=\frac1{r\sin\theta}\left[\partial_\theta(\sin\theta F_\phi)-\partial_\phi F_\theta\right]
=\frac{(m+1)\cos\theta\sin\phi}{r^2\sin\theta}.
$$

It vanishes identically exactly when **$m=-1$**. In that case integrate $F_\theta=-r^{-1}V_\theta$ to obtain $V=-\sin\theta\cos\phi+C(\phi)$. The azimuthal equation $F_\phi=-(r\sin\theta)^{-1}V_\phi$ forces $C'\!=0$, and $F_r=0$ removes any radial dependence. At the given north-pole point the first term is zero, so normalization fixes the constant to zero:

$$
\boxed{V=-\sin\theta\cos\phi=-\frac{x}{\sqrt{x^2+y^2+z^2}}.}
$$

The Cartesian expression shows that this potential and the field $\mathbf F=\nabla(x/r)$ are smooth for $r>0$, including the spherical-coordinate poles. The origin is excluded because the specified field is singular there; that exclusion does not obstruct the displayed global potential.

## ↑ Ancestors (10)

1. [3B](../3b.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ia](../../split.md)
4. [2009](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
