<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

The Lorenz equilibria satisfy $y=x$, $z=x^2/b$ and $x(r-1-z)=0$. Thus

$$
\boxed{O=(0,0,0),\qquad C_\pm=(\pm\sqrt{b(r-1)},\pm\sqrt{b(r-1)},r-1)\quad(r>1).}
$$

At the origin the third [eigenvalue](../../../../eigenvalue.md) is $-b$ and the other two solve $\lambda^2+(\sigma+1)\lambda+\sigma(1-r)=0$. Hence the origin is stable for $r<1$, has one zero [eigenvalue](../../../../eigenvalue.md) at $r=1$, and becomes a [saddle equilibrium](../../../../saddle-equilibrium.md) with one unstable direction for $r>1$. The [symmetry](../../../../symmetry-physics.md) $(x,y,z)\mapsto(-x,-y,z)$ interchanges the new branches.

The nonzero-equilibrium characteristic polynomial is

$$
\boxed{P(\lambda)=\lambda^3+(\sigma+b+1)\lambda^2+b(\sigma+r)\lambda+2\sigma b(r-1).}
$$

Near $r=1$ its Routh-Hurwitz inequalities are strict, so both new branches are stable. More explicitly, center-manifold projection at $r=1$ gives

$$
\dot q=\frac\sigma{\sigma+1}(r-1)q-\frac\sigma{b(\sigma+1)}q^3+
O((r-1)^2q,(r-1)q^3,q^5).
$$

The linear coefficient crosses positively and the cubic coefficient is negative. Therefore **the equilibrium [bifurcation](../../../../bifurcation.md) is a supercritical pitchfork at $r=1$**, not a [saddle equilibrium](../../../../saddle-equilibrium.md)-node.

For completeness, the later stability boundary satisfies

$$
(\sigma+b+1)(\sigma+r)=2\sigma(r-1).
$$

If $\sigma\leq b+1$, the nonzero branches remain linearly stable for all $r>1$. If $\sigma>b+1$, they lose stability at

$$
\boxed{r_H=\frac{\sigma(\sigma+b+3)}{\sigma-b-1},\qquad
\omega_H^2=b(\sigma+r_H).}
$$

At that point $P=(\lambda+\sigma+b+1)(\lambda^2+\omega_H^2)$ and

$$
\left.\frac{d\operatorname{Re}\lambda}{dr}\right|_H
=\frac{b(\sigma-b-1)}{2[\omega_H^2+(\sigma+b+1)^2]}>0.
$$

This establishes a genuine transverse Hopf crossing. It is **subcritical** for these positive [parameters](../../../../parameter.md), so it is not the supercritical Hopf [normal form of a dynamical system](../../../../normal-form-dynamical-systems.md) from (c). One way to check its nonlinear sign is the cubic Hopf formula. At $C_+$ write $s=\sqrt{b(r_H-1)}$ and

$$
A=\begin{pmatrix}-\sigma&\sigma&0\\1&-1&-s\\s&s&-b\end{pmatrix},\qquad
B(v,w)=(0,-v_1w_3-v_3w_1,v_1w_2+v_2w_1).
$$

For right and adjoint eigenvectors $Aq=i\omega_Hq$, $A^*p=-i\omega_Hp$, $\langle p,q\rangle=1$, the cubic coefficient has the sign of

$$
\operatorname{Re}\langle p,
B(\bar q,(2i\omega_HI-A)^{-1}B(q,q))
-2B(q,A^{-1}B(q,\bar q))\rangle.
$$

Substitution and clearing positive factors reduces its sign to that of the following polynomial in $h=\sigma-b-1>0$:

$$
9h^4+2(9b+28)h^3+4(5b^2+29b+31)h^2+
4(b+1)(b+2)(5b+14)h+8(b+1)^2(b+2)^2.
$$

Every term is positive. The radial cubic is therefore positive, giving the unstable small cycle on the stable-equilibrium side. There is no [saddle equilibrium](../../../../saddle-equilibrium.md)-node among the equilibrium branches for $\sigma,b,r>0$: the only zero-[eigenvalue](../../../../eigenvalue.md) branch intersection is the [symmetry](../../../../symmetry-physics.md)-forced pitchfork. This does not rule out separate global [bifurcations](../../../../bifurcation.md) of [periodic orbits](../../../../periodic-orbit.md).

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2007](../../../2007-split.md)
4. [Past exam of the topics in applied mathematics course of the University of Oxford](../../../split.md)
5. [Topics in applied mathematics course of the University of Oxford](../../../../topics-in-applied-mathematics-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
