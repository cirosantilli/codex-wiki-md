<h1 id="3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

The map

$$
[i](x,y)=(-x,iy)
$$

is an automorphism of the [elliptic curve](../../../../../elliptic-curve.md) over $K$, fixes its identity point, and squares to $[-1]$. For the [invariant differential on an elliptic curve](../../../../../invariant-differential-on-an-elliptic-curve.md) $\omega=dx/(2y)$, it satisfies $[i]^*\omega=i\omega$. Thus $\mathbb Z[i]\subseteq\operatorname{End}_K(E)$, with the indicated embedding of $K$.

Under analytic [complex uniformization of an elliptic curve](../../../../../complex-uniformization-of-an-elliptic-curve.md) $E(\mathbb C)\simeq\mathbb C/L$, this automorphism acts as multiplication by $i$, so $L$ is stable under $\mathbb Z[i]$. It is a rank-one torsion-free [module](../../../../../module-mathematics.md) over the [Gaussian integers](../../../../../gaussian-integer.md). Since that [ring](../../../../../ring.md) is a [principal ideal domain](../../../../../principal-ideal-domain.md), $L=\Omega\mathbb Z[i]$. Every analytic [endomorphism](../../../../../endomorphism.md) is multiplication by an $a\in\mathbb C$ with $aL\subseteq L$, which here says exactly $a\in\mathbb Z[i]$. Therefore the geometric [endomorphism ring of an elliptic curve](../../../../../endomorphism-ring-of-an-elliptic-curve.md) is $\mathbb Z[i]$, and all its elements are generated over $\mathbb Z$ by the displayed $K$-defined automorphism. Thus $\operatorname{End}_K(E)=\mathbb Z[i]$.

If an [endomorphism](../../../../../endomorphism.md) is defined over $\mathbb Q$, its pullback on the rational differential $\omega$ has scalar in $\mathbb Q$. The differential action is injective in characteristic zero, because a nonzero [isogeny of elliptic curves](../../../../../isogeny-of-elliptic-curves.md) is separable and has nonzero differential. Its scalar must therefore lie in $\mathbb Q\cap\mathbb Z[i]=\mathbb Z$. Conversely integer multiplication is defined over $\mathbb Q$. Hence

$$
\boxed{\operatorname{End}_{\mathbb Q}(E)=\mathbb Z,\qquad\operatorname{End}_{\mathbb Q(i)}(E)=\mathbb Z[i].}
$$

Put $\lambda=1+i$. The valuations of the differences of the three nonidentity fourth roots of unity from $1$ are

$$
v_\lambda(-1-1)=2,\qquad v_\lambda(i-1)=1,\qquad v_\lambda(-i-1)=1.
$$

For instance $2=-i\lambda^2$, and the other two differences are associates of $\lambda$. None is divisible by $\lambda^3$. The group $(\mathbb Z[i]/\lambda^3)^\times$ has $8-4=4$ elements, so the four units map bijectively to it. Every ideal prime to $\lambda$ consequently has a unique [primary Gaussian integer](../../../../../primary-gaussian-integer.md) generator.

The [Grössencharacter of the square-lattice elliptic curve](../../../../../grossencharacter-of-the-square-lattice-elliptic-curve.md) is explicitly

$$
\boxed{\psi_E(\mathfrak a)=\alpha,\qquad(\alpha)=\mathfrak a,\quad\alpha\equiv1\pmod{\lambda^3},\qquad\mathfrak f=\lambda^3.}
$$

For integral ideals prime to $2$, the generator is an odd [Gaussian integer](../../../../../gaussian-integer.md); extend multiplicatively to fractional ideals prime to $2$. Products of primary generators are primary, so this is a [Hecke character](../../../../../hecke-character.md) with ideal infinity type $(1,0)$: on a principal ideal with generator $a\equiv1\pmod{\lambda^3}$, its value is $a$. Its conductor divides $\lambda^3$, and cannot divide $\lambda^2$, since $-1\equiv1\pmod{\lambda^2}$ would force $\psi_E(({-1}))=-1$, whereas the unit ideal has value $1$. Thus the displayed conductor is exact.

We next verify directly that this character gives the Frobenius values of this particular curve, fixing the unit ambiguity. The point

$$
P=(i,1-i)\in E(K)
$$

satisfies, by the chord-and-tangent addition law,

$$
[\lambda]P=(1,0),\qquad[\lambda]^2P=(0,0),\qquad[\lambda]^3P=O.
$$

For the first addition, $[i]P=(-i,1+i)$ and the chord has slope $-1$. Since $P$ is killed by $\lambda^3$ but not by $\lambda^2$, it generates the eight-element $\mathbb Z[i]$-module $E[\lambda^3]\simeq\mathbb Z[i]/\lambda^3$. Thus all this torsion is rational over $K$.

The model has discriminant $64$, so it has [good reduction](../../../../../good-reduction-of-an-elliptic-curve.md) at every $\gamma\ne(\lambda)$. First suppose $\gamma$ lies over a split rational prime $p$. Then its residue field is $\mathbb F_p$, $p\geq5$, and $\pi=\psi_E(\gamma)$ has norm $p$. Reduction of $[\pi]$ still has degree $p$ and has zero differential, since its differential scalar $\pi$ belongs to $\gamma$. It is therefore purely inseparable of degree $p$. Factoring out the [Frobenius isogeny](../../../../../frobenius-isogeny-of-an-elliptic-curve.md) gives

$$
\widetilde{[\pi]}=u\circ\operatorname{Frob}_p
$$

for an automorphism $u$ of the reduction. In characteristic at least five, the automorphisms of this model fixing $O$ are the four Gaussian units: comparing coefficients in $(x,y)\mapsto(v^2x,v^3y)$ gives $v^4=1$. Prime-to-$p$ torsion reduces injectively. Both $[\pi]$ and $\operatorname{Frob}_p$ fix the reduction of $E[\lambda^3]$, the former by the primary congruence and the latter by its rationality over the residue field. Thus $u$ fixes this entire module. The unit congruences proved above force $u=1$.

For an inert rational prime $p\equiv3\pmod4$, we have $\gamma=(p)$, $N\gamma=p^2$, and its primary generator is $\pi=-p$, because $4\mid p+1$ implies $\lambda^3\mid(-p-1)$. To determine Frobenius without excluding $p=3$, write

$$
a_p=-\sum_{x\in\mathbb F_p}\left(\frac{x^3-x}{p}\right).
$$

Replacing $x$ by $-x$ changes each nonzero quadratic-character value to its negative, because $-1$ is a nonsquare. Hence $a_p=0$. The Frobenius characteristic equation $\operatorname{Frob}_p^2-[a_p]\operatorname{Frob}_p+[p]=0$ gives $\operatorname{Frob}_{p^2}=[-p]$. This proves the asserted Frobenius value at inert primes as well, and identifies the displayed [Hecke character](../../../../../hecke-character.md) with that of $E$.

Finally, the formal parameter $t=-x/y$ is defined over the local [ring](../../../../../ring.md) at $\gamma$. Since the reduced [endomorphism](../../../../../endomorphism.md) is the $q$-power [Frobenius isogeny](../../../../../frobenius-isogeny-of-an-elliptic-curve.md), with $q=N\gamma$, its pullback sends $t$ to $(-x/y)^q=t^q$. Passing to the completion at the identity gives the equality of formal series

$$
\boxed{[\pi](t)\equiv t^{N\gamma}\pmod\gamma.}
$$

## ↑ Ancestors (10)

1. [3](../3.md)
2. [Paper 23](../../paper-23-split.md)
3. [Iii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
