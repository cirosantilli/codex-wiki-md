<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

For a rank-$r$ real [vector bundle](../../../../../vector-bundle.md) with a [fiber metric](../../../../../fiber-metric.md), the [Thom isomorphism theorem](../../../../../thom-isomorphism-theorem.md) says that if the bundle is oriented over the coefficient ring $R$, there is a [Thom class](../../../../../thom-class.md) $u\in H^r(D(E),S(E);R)$ restricting to the chosen generator on every fiber pair, and

$$
H^q(B;R)\xrightarrow{\ \pi^*(-)\smile u\ }H^{q+r}(D(E),S(E);R)
$$

is an isomorphism. For $R=\mathbb F_2$, every real vector bundle has the required orientation. The disk bundle retracts to $B$, so apply the pair long exact sequence and the Thom isomorphism to get the [Gysin sequence of a sphere bundle](../../../../../gysin-sequence-of-a-sphere-bundle.md)

$$
\boxed{\cdots\to H^{q-r}(B;R)\xrightarrow{\smile e(E)}H^q(B;R)\xrightarrow{\pi^*}H^q(S(E);R)\xrightarrow{\pi_!}H^{q-r+1}(B;R)\xrightarrow{\smile e(E)}H^{q+1}(B;R)\to\cdots.}
$$

The first map is multiplication by the [Euler class of a vector bundle](../../../../../euler-class-of-a-vector-bundle.md), the pullback to the zero section of the absolute image of $u$. The connecting map followed by inverse Thom isomorphism gives $\pi_!$.

Apply this over $\mathbb F_2$ to the tautological real line bundle $\gamma$ on $\mathbb{RP}^n$. Its unit sphere bundle is $S^n$, with projection sending a unit vector to its line. Put $a=e_2(\gamma)=w_1(\gamma)\in H^1(\mathbb{RP}^n;\mathbb F_2)$, the [mod-two Euler class of a real line bundle](../../../../../mod-two-euler-class-of-a-real-line-bundle.md). For $n\geq1$ the degree-zero pullback $H^0(\mathbb{RP}^n)\to H^0(S^n)$ is an isomorphism. Exactness therefore makes the subsequent transfer zero, and multiplication by $a$ from $H^0$ into $H^1$ injective. In intermediate degrees the sphere cohomology vanishes, making each successive multiplication by $a$ an isomorphism. At degree $n$, the map from $H^{n-1}$ into $H^n$ is injective; the transfer $H^n(S^n)\to H^n(\mathbb{RP}^n)$ is surjective because $H^{n+1}(\mathbb{RP}^n)=0$. Since $H^n(S^n)=\mathbb F_2$, that top group is one-dimensional too, and $a^n$ is its nonzero generator. The same endpoint reasoning covers $n=1$. This gives the [Gysin proof of mod-two projective-space cohomology](../../../../../gysin-proof-of-mod-two-projective-space-cohomology.md) and the [mod-two cohomology ring of real projective space](../../../../../mod-two-cohomology-ring-of-real-projective-space.md):

$$
\boxed{H^*(\mathbb{RP}^n;\mathbb F_2)=\mathbb F_2[a]/(a^{n+1}),\qquad|a|=1.}
$$

For $n=0$ this says simply $H^*(\mathbb{RP}^0)=\mathbb F_2$.

For a self-map of $\mathbb{RP}^4$, the induced map has $f^*a=\lambda a$ with $\lambda\in\mathbb F_2$, so $f^*a^j=\lambda^j a^j$. The mod-two alternating trace is

$$
L_2(f)=1+\lambda+\lambda^2+\lambda^3+\lambda^4=1
$$

for either value of $\lambda$. The alternating trace on homology equals that on the finite cellular chain complex; consequently this is the reduction modulo two of the integral [Lefschetz number](../../../../../lefschetz-number.md). That integer is nonzero, and the [Lefschetz fixed-point theorem](../../../../../lefschetz-fixed-point-theorem.md) forces a fixed point. Thus **every self-map of the real projective four-space has a fixed point**, a case of the [Lefschetz fixed-point property of even-dimensional real projective space](../../../../../lefschetz-fixed-point-property-of-even-dimensional-real-projective-space.md).

For the odd-dimensional example, let $J(x_1,x_2,x_3,x_4)=(-x_2,x_1,-x_4,x_3)$, so $J^2=-I$. Its projectivization is

$$
\boxed{F([x_1:x_2:x_3:x_4])=[-x_2:x_1:-x_4:x_3].}
$$

It is well-defined and continuous on $\mathbb{RP}^3$. A fixed projective point would have $Jv=tv$ for a nonzero real vector and real $t$, forcing $-v=J^2v=t^2v$ and therefore $t^2=-1$, impossible. This is a [fixed-point-free complex-structure map on odd-dimensional real projective space](../../../../../fixed-point-free-complex-structure-map-on-odd-dimensional-real-projective-space.md).

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
