<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put $\widetilde\xi_t=\phi_t(\xi_t)$ and $p_t=\phi_t'(\xi_t)$. The given [conformal change of half-plane capacity](../../../../../../conformal-change-of-half-plane-capacity.md) makes the image mapping-out equation

$$
\partial_t\widetilde g_t(w)
=\frac{2p_t^2}{\widetilde g_t(w)-\widetilde\xi_t}.
$$

Indeed its capacity speed is $2p_t^2$, and the stated [Loewner local growth property](../../../../../../loewner-local-growth-property.md) identifies the indicated single driver. For $t<T$, differentiate the conjugacy identity

$$
\widetilde g_t\circ\phi=\phi_t\circ g_t
$$

at a fixed original point. The [Chordal Loewner equation](../../../../../../chordal-loewner-equation.md) then gives the **[conformal conjugacy derivative for the chordal Loewner equation](../../../../../../conformal-conjugacy-derivative-for-the-chordal-loewner-equation.md)**

$$
\boxed{\dot\phi_t(z)
=\frac{2\phi_t'(\xi_t)^2}{\phi_t(z)-\phi_t(\xi_t)}
-\frac{2\phi_t'(z)}{z-\xi_t}.}
$$

The change of variable $z=g_t(w)$ covers the whole upper half-plane. The [conformal automorphism of the upper half-plane](../../../../../../conformal-automorphism-of-the-upper-half-plane.md) $\phi_t$ is a real [Möbius transformation](../../../../../../mobius-transformation.md). Its pole is the image of the still-unswallowed boundary point $-1$, so it is holomorphic in a neighbourhood of $\xi_t$ before $T$.

To evaluate the apparent singularity, write $h=z-\xi_t$, $p=\phi_t'(\xi_t)>0$ and $q=\phi_t''(\xi_t)$. The [Taylor series](../../../../../../taylor-series.md) is

$$
\phi_t(\xi_t+h)-\phi_t(\xi_t)=ph+\tfrac12qh^2+O(h^3),
\qquad\phi_t'(\xi_t+h)=p+qh+O(h^2).
$$

Thus the first term in the derivative is $2p/h-q+O(h)$, while the second is $2p/h+2q+O(h)$. Their poles cancel and their constant terms differ by $-3q$. Therefore

$$
\boxed{\dot\phi_t(\xi_t)=-3\phi_t''(\xi_t).}
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 203](../../../paper-203-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
