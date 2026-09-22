<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

For a single [chiral superfield](../../../../../chiral-superfield.md), the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md), with $\kappa=m_p^{-1}$ restored, is

$$
V=e^{\kappa^2K}\left(K^{z\bar z}|D_zW|^2-3\kappa^2|W|^2\right),
\qquad D_zW=W_z+\kappa^2K_zW.
$$

The canonical [Kähler potential](../../../../../kahler-potential.md) has $K_{z\bar z}=K^{z\bar z}=1$, so the [Kähler covariant derivative of a superpotential](../../../../../kahler-covariant-derivative-of-a-superpotential.md) is

$$
D_zW=\mu m_p\left[1+\kappa^2\bar z(z+\beta)\right].
$$

Consequently the [Polonyi model](../../../../../polonyi-model.md) has the [scalar potential](../../../../../scalar-potential.md)

$$
\boxed{V=|\mu|^2m_p^2e^{\kappa^2|z|^2}
\left(\left|1+\kappa^2\bar z(z+\beta)\right|^2
-3\kappa^2|z+\beta|^2\right).}
$$

The negative term is essential; retaining only the square of the [supergravity auxiliary field](../../../../../supergravity-auxiliary-field.md) would give the global [F-term scalar potential](../../../../../f-term-scalar-potential.md) rather than the [supergravity F-term potential](../../../../../supergravity-f-term-potential.md).

Set $x=\kappa z=a+iy$ and $b=\kappa\beta=2-\sqrt3$. In this notation $V=|\mu|^2m_p^2e^{|x|^2}U$, where

$$
U=\left(1+a^2+y^2+ba\right)^2+b^2y^2
-3\left[(a+b)^2+y^2\right].
$$

At $a_0=\sqrt3-1$, $y=0$, one has $a_0+b=1$ and $1+a_0(a_0+b)=\sqrt3$, so $U=0$. To prove that this is a [local minimum](../../../../../local-minimum.md) in both real directions, rather than checking only the real axis, put $u=a-a_0$. Direct expansion gives the [stable zero-energy Polonyi vacuum](../../../../../stable-zero-energy-polonyi-vacuum.md) identity

$$
U=\left(u^2+y^2+\sqrt3u\right)^2
+(2\sqrt3-3)u^2+(4-2\sqrt3)y^2.
$$

Every coefficient outside the square is strictly positive, and the exponential factor is positive. Thus $V\ge0$ everywhere and equality requires $u=y=0$, provided $\mu\ne0$. This proves the stronger conclusion

$$
\boxed{\langle z\rangle=(\sqrt3-1)m_p,\qquad V_{\min}=0,}
$$

a unique [global minimum](../../../../../global-minimum.md) of this [Polonyi model](../../../../../polonyi-model.md). If $\mu=0$, the [scalar potential](../../../../../scalar-potential.md) vanishes identically and this uniqueness and [supersymmetry breaking](../../../../../supersymmetry-breaking.md) conclusion do not hold.

For an independent local stability check, the [Hessian matrix](../../../../../hessian-matrix.md) of $U$ at this [global minimum](../../../../../global-minimum.md) is diagonal:

$$
U_{aa}=4\sqrt3,\qquad U_{yy}=8-4\sqrt3,\qquad U_{ay}=0.
$$

Since $U$ and its first derivatives vanish there, differentiating the exponential introduces no additional [Hessian matrix](../../../../../hessian-matrix.md) terms at the [global minimum](../../../../../global-minimum.md). For canonically normalized real fluctuations $z=z_0+(s+it)/\sqrt2$, the squared scalar [masses](../../../../../mass.md) are therefore

$$
m_s^2=2\sqrt3\,|\mu|^2e^{a_0^2},
\qquad
m_t^2=2(2-\sqrt3)|\mu|^2e^{a_0^2},
$$

which are both positive.

Although the vacuum energy is zero, the [supergravity auxiliary field](../../../../../supergravity-auxiliary-field.md) is not. In the convention $F^z=-e^{\kappa^2K/2}\overline{D_zW}$, its [vacuum expectation value](../../../../../vacuum-expectation-value.md) obeys

$$
|F^z|=\sqrt3\,|\mu|m_p e^{a_0^2/2}\ne0.
$$

The matter [fermion](../../../../../fermion.md) transformation contains a term proportional to $F^z\epsilon$, so no nonzero constant [supersymmetry](../../../../../supersymmetry-split.md) parameter leaves this vacuum invariant. Hence **supersymmetry is spontaneously broken even though the vacuum energy vanishes**: the positive [auxiliary field](../../../../../auxiliary-field.md) contribution cancels the negative gravitational term. The matter [fermion](../../../../../fermion.md) supplies the [goldstino](../../../../../goldstino.md), which is absorbed by the [gravitino](../../../../../gravitino.md) in the [super-Higgs mechanism](../../../../../super-higgs-mechanism.md).

Using the [gravitino mass from a superpotential](../../../../../gravitino-mass-from-a-superpotential.md), and $z_0+\beta=m_p$, gives

$$
\boxed{m_{3/2}=\kappa^2 e^{\kappa^2K/2}|W|
=|\mu|e^{2-\sqrt3}
=\frac{|F^z|}{\sqrt3m_p}.}
$$

An [auxiliary field](../../../../../auxiliary-field.md) $F^z$ has [mass dimension](../../../../../mass-dimension.md) two. Defining the [supersymmetry breaking](../../../../../supersymmetry-breaking.md) scale by $\Lambda_{\mathrm{SUSY}}=\sqrt{|F^z|}$, one obtains

$$
\frac{m_{3/2}}{\Lambda_{\mathrm{SUSY}}}
=\frac{\Lambda_{\mathrm{SUSY}}}{\sqrt3m_p}.
$$

Thus the [gravitino](../../../../../gravitino.md) [mass](../../../../../mass.md) is small compared with the [supersymmetry breaking](../../../../../supersymmetry-breaking.md) scale when that scale is sub-Planckian, as in the usual hierarchy $|\mu|\ll m_p$. This smallness is gravitational suppression; it is not a conclusion valid for arbitrary choices of the mass parameter.

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
