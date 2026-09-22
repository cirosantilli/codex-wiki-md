<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take two [solid tori](../../../../../../solid-torus.md) $V_1,V_2$, each with a meridian-longitude [basis](../../../../../../basis.md) $(\mu_i,\lambda_i)$ on its boundary. Use opposite boundary-basis orientations on the two sides, so that a determinant-one coefficient matrix describes an [orientation](../../../../../../orientation-of-a-simplex.md)-reversing gluing map. For $A\in SL(2,\mathbb Z)$ choose a torus [homeomorphism](../../../../../../homeomorphism.md) $f:\partial V_2\to\partial V_1$ inducing

$$
f_*\mu_2=-q\mu_1+p\lambda_1,\qquad
f_*\lambda_2=s\mu_1+r\lambda_1,
$$

and define $M_A=V_1\cup_fV_2$. The linear map on $\mathbb R^2/\mathbb Z^2$ realizes the matrix. Torus [homeomorphisms](../../../../../../homeomorphism.md) with the same action on [first homology](../../../../../../first-homology.md) are isotopic, and an isotopy extends over a boundary collar, so the resulting [three-manifold](../../../../../../3-manifold.md) depends only on $A$. Specifying opposite boundary conventions is necessary: gluing two identically oriented boundary bases by a determinant-one map would not describe the usual oriented gluing.

We now identify this gluing directly in the quotient from part (a). Split $S^3$ into the two invariant [solid tori](../../../../../../solid-torus.md) $W_1=\{|z_2|\le1/\sqrt2\}$ and $W_2=\{|z_1|\le1/\sqrt2\}$. On $W_1$ write $z_1=\sqrt{1-|w|^2}e^{2\pi ix}$, $z_2=w$. The quotient coordinates

$$
(u,v)=(e^{2\pi ipx},e^{-2\pi iqx}w)
$$

identify $W_1/\langle g\rangle$ with $S^1\times D^2$. They are invariant under $g$; choosing a $p$th root of $u$ reconstructs $(x,w)$, and different choices are exactly the same cyclic orbit. Thus this is a genuine solid-torus coordinate model.

On the common boundary, measure arguments in turns as $(x,y)$. Its quotient lattice is

$$
\mathcal L=\mathbb Z^2+\mathbb Z(1/p,q/p).
$$

The meridian and longitude of the first quotient torus can be chosen as $\mu_1=(0,1)$ and $\lambda_1=(1/p,q/p)$. They form a lattice [basis](../../../../../../basis.md), since $(1,0)=p\lambda_1-q\mu_1$. The meridian of the second torus is precisely that $(1,0)$ loop. Consequently

$$
\boxed{\mu_2=-q\mu_1+p\lambda_1.}
$$

The determinant condition is $qr+ps=-1$. Put $k=-r$, so $kq\equiv1\pmod p$. On $W_2$, the analogous quotient coordinates use $e^{2\pi ipy}$ and $e^{-2\pi iky}z_1$, and a longitude is $(k/p,1/p)$. Choose its negative for the second boundary-basis convention. Then

$$
\lambda_2=(-k/p,-1/p)=s\mu_1+r\lambda_1,
$$

since $ps+qr=-1$. Thus the two quotient tori are glued by exactly $A$. This proves the [genus-one gluing model of a lens space](../../../../../../genus-one-gluing-model-of-a-lens-space.md) and

$$
\boxed{M_A\cong L(p,q).}
$$

Different choices of $r,s$ satisfying the determinant condition differ by $(s,r)\mapsto(s,r)+j(-q,p)$. This changes $f$ by a meridional [Dehn twist](../../../../../../dehn-twist.md) on $V_2$, which extends over $V_2$: in solid-torus coordinates it is $(z,e^{i\theta})\mapsto(e^{ij\theta}z,e^{i\theta})$. Therefore there is no hidden dependence on that choice of longitude.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 24](../../../paper-24-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
