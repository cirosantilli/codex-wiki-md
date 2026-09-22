<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $\Lambda=H^2(X,\mathbb Z)$ with the cup-product pairing $q$ of signature $(3,19)$. For a [K3 surface](../../../../../../k3-surface.md), the [Hodge numbers](../../../../../../hodge-number.md) are $(h^{2,0},h^{1,1},h^{0,2})=(1,20,1)$. A nonzero holomorphic two-form $\omega$ spans $F^2$, and its wedge products give

$$
q(\omega,\omega)=0,\qquad q(\omega,\bar\omega)>0.
$$

The remaining filtration is forced by orthogonality:

$$
F^2=\mathbb C\omega,\qquad F^1=\omega^\perp,
\qquad H^{1,1}=(\mathbb C\omega\oplus\mathbb C\bar\omega)^\perp.
$$

Thus the usual [K3 period domain](../../../../../../k3-period-domain.md) and its quadric compactification are

$$
\check D_\Lambda=\{[\omega]\in\mathbb P(\Lambda_{\mathbb C}):
q(\omega,\omega)=0\},\qquad
D_\Lambda=\{[\omega]\in\check D_\Lambda:q(\omega,\bar\omega)>0\}.
$$

The quadric is smooth and has complex dimension $21-1=20$. Writing $\omega=x+iy$, its equations say that $x,y$ are orthogonal positive vectors of equal square. A period therefore determines an oriented positive two-plane in $\Lambda_{\mathbb R}$.

There is a polarization qualification: the full cup-product form is not a polarization in the strict sense of part (a). Its real $(1,1)$ space has signature $(1,19)$, so it cannot satisfy the negative-definiteness requirement there. Fixing an ample integral class $h$ of square $2d>0$ and requiring it to stay of type $(1,1)$ gives the [primitive cohomology](../../../../../../primitive-cohomology.md) lattice

$$
\Lambda_h=h^\perp,\qquad \operatorname{signature}(\Lambda_h)=(2,19).
$$

Its genuine polarized [Griffiths domain](../../../../../../period-domain.md) is

$$
\boxed{D_h=\{[\omega]\in\mathbb P((\Lambda_h)_{\mathbb C}):
q(\omega,\omega)=0,\ q(\omega,\bar\omega)>0\}.}
$$

Its compact dual is the corresponding smooth quadric of complex dimension nineteen, and $D_h$ has two components, distinguished by the orientation of the positive two-plane. For ample-polarized geometric K3 moduli one also removes the loci $(\omega,\delta)=0$ with $\delta\in\Lambda_h$, $\delta^2=-2$, since an ample class cannot be orthogonal to an effective rational curve. Those exclusions concern the ample moduli locus; they are not part of the definition of the polarized Hodge domain.

If one wants a strict polarization on the full $H^2$ of a fixed projective surface, reverse the sign on its rational Kähler line and retain $q$ on the orthogonal complement. For example the integral form

$$
Q_h(u,v)=q(h,h)q(u,v)-2q(u,h)q(v,h)
$$

has the required positivity and signature $(2,20)$. It is a different form from the [cup product](../../../../../../cup-product.md). The twenty-dimensional full period quadric and the nineteen-dimensional primitive polarized domain should therefore be distinguished. The positivity and signature calculations above explain why these two domains describe different data.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 21](../../../paper-21-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
