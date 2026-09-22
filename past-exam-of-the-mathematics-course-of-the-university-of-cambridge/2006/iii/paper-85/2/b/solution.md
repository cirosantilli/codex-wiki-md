<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The origin's [Jacobian matrix](../../../../../../jacobian-matrix.md) is triangular, $J=\begin{pmatrix}a+1&1\\0&b-1\end{pmatrix}$, so its [Floquet multipliers](../../../../../../floquet-multiplier.md) are $a+1$, $b-1$. It is attracting for $-2<a<0$, $0<b<2$. The candidate codimension-one boundaries are $a=0$, $a=-2$, $b=2$, $b=0$: respectively a $+1$ or $-1$ [Floquet multiplier](../../../../../../floquet-multiplier.md). No complex-pair crossing is possible at the origin.

The map is odd. To locate the nearby steady branches, write $S=x^2>0$. The first fixed-point equation gives $y=x(S-a)$; substituting into the second gives

$$
\boxed{S[1-(S-a)^3]=a(2-b).}
$$

For a symmetric [two-cycle](../../../../../../period-two-orbit.md) solve $F(x,y)=-(x,y)$. Then $y=x(S-a-2)$ and

$$
\boxed{S[1+(S-a-2)^3]=b(a+2).}
$$

These exact [orbit equations for a triangular cubic map](../../../../../../orbit-equations-for-a-triangular-cubic-map.md) determine the [amplitude](../../../../../../wave-amplitude.md) and parameter side without confusing the original cubic coefficients with their [centre manifold](../../../../../../center-manifold.md) values.

On $a=0$, with $b\ne2$, steady states have $x^2=a(2-b)+o(a)$ and $y=-ax+x^3$. The [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) is supercritical for $b<2$ and subcritical for $b>2$. Its [centre manifold](../../../../../../center-manifold.md) cubic coefficient is $-1/(2-b)$. In the stable-origin boundary segment $0<b<2$, an attracting pair appears on $a>0$.

On $a=-2$, with $b\ne0$, the [two-cycle](../../../../../../period-two-orbit.md) has $x^2=b(a+2)+o(a+2)$. The [centre manifold](../../../../../../center-manifold.md) map has cubic coefficient $-1/b$ and [Floquet multiplier](../../../../../../floquet-multiplier.md) $-1+(a+2)$. Since its unstable side is $a+2<0$, the [period-doubling bifurcation](../../../../../../period-doubling-bifurcation.md) is supercritical for $b<0$ and subcritical for $b>0$. In particular the boundary segment $0<b<2$ is subcritical: the nearby [two-cycle](../../../../../../period-two-orbit.md) lies on $a>-2$, where the origin is still attracting, and is unstable in the critical direction.

On $b=2$, with $a\ne0$, the steady branch has

$$
y^2\sim-\frac{a^3}{1+a^3}(b-2).
$$

Its scalar [centre manifold](../../../../../../center-manifold.md) map is $y'=(1+b-2)y+(1+a^{-3})y^3+\cdots$. It is supercritical for $-1<a<0$, and subcritical for $a<-1$ or $a>0$. At $a=-1$ the cubic vanishes: the exact equation gives $b-2=-3S^2+O(S^3)$, so this is a degenerate [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) with destabilizing quintic coefficient and subcritical quartic [amplitude](../../../../../../wave-amplitude.md) scaling. It is not a generic point of the codimension-one curve.

On $b=0$, with $a\ne-2$, put $A=a+2$. The [two-cycle](../../../../../../period-two-orbit.md) satisfies

$$
y^2\sim\frac{A^3}{1-A^3}b.
$$

The [centre manifold](../../../../../../center-manifold.md) map's cubic coefficient is $1-A^{-3}$. Thus the [period-doubling bifurcation](../../../../../../period-doubling-bifurcation.md) is subcritical for $-2<a<-1$, and supercritical for $a<-2$ or $a>-1$. In the stable-origin edge $-1<a<0$, a stable small [two-cycle](../../../../../../period-two-orbit.md) appears for $b<0$. At $a=-1$ the cubic vanishes, requiring the calculation below. All criticality labels concern the [centre manifold](../../../../../../center-manifold.md) direction; a bifurcating orbit is fully attracting only if the remaining [Floquet multiplier](../../../../../../floquet-multiplier.md) is also stable. The sketch marks the small branches on the appropriate sides of each boundary of the stable-origin rectangle.

For clarity, these stability labels follow directly from one-dimensional [derivatives](../../../../../../derivative.md). At a [pitchfork bifurcation](../../../../../../pitchfork-bifurcation-normal-form.md) $z'=(1+\eta)z+cz^3$, the nonzero state has $z^2=-\eta/c$ and [Floquet multiplier](../../../../../../floquet-multiplier.md) $1-2\eta$ to first order. At a [period-doubling bifurcation](../../../../../../period-doubling-bifurcation.md) $z'=-(1+\eta)z+cz^3$, the symmetric cycle has $z^2=\eta/c$ and one-step [derivative](../../../../../../derivative.md) $-1+2\eta$; its two-step [Floquet multiplier](../../../../../../floquet-multiplier.md) is $1-4\eta+o(\eta)$. A supercritical branch lies on $\eta>0$ and is attracting in the [centre manifold](../../../../../../center-manifold.md) direction; a subcritical branch lies on $\eta<0$ and is repelling there.

At $(a,b)=(-1,0)$ the [Floquet multipliers](../../../../../../floquet-multiplier.md) are $0,-1$, so the degeneracy is not two simultaneous unit [Floquet multipliers](../../../../../../floquet-multiplier.md). On its [centre manifold](../../../../../../center-manifold.md), $x=-y-y^3+O(y^7)$ and direct substitution gives $y'=-y-3y^5+O(y^7)$. With $\alpha=a+1$ small, the unfolding to leading weighted order is

$$
\boxed{y'=(-1+b)y+3\alpha y^3-3y^5+\cdots.}
$$

This is a [generalized flip bifurcation](../../../../../../generalized-flip-bifurcation.md): one parameter crosses $-1$, and the other changes the cubic sign. Writing $S\simeq y^2$, its [two-cycles](../../../../../../period-two-orbit.md) obey $b+3\alpha S-3S^2=0$. For $\alpha>0$ a stable smaller [two-cycle](../../../../../../period-two-orbit.md) and an unstable larger [two-cycle](../../../../../../period-two-orbit.md) collide at

$$
\boxed{b=-\tfrac34\alpha^2+o(\alpha^2),\qquad S=\tfrac12\alpha+o(\alpha).}
$$

The intervening range $-3\alpha^2/4<b<0$ contains both. For $\alpha<0$ the [period-doubling bifurcation](../../../../../../period-doubling-bifurcation.md) is subcritical. At $\alpha=0$, the exact orbit equation is $3S^2-3S^3+S^4=b$, so the unstable [two-cycle](../../../../../../period-two-orbit.md) exists for $b>0$ with $|y|\sim(b/3)^{1/4}$. This proves both the codimension and the required quintic effect.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 85](../../../paper-85-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
