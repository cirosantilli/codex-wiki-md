<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

We first derive the exterior [area theorem for univalent functions](../../../../../area-theorem-conformal-mapping.md) directly from [Green's theorem](../../../../../green-theorem.md), then obtain the coefficient bound needed for the [Koebe quarter theorem](../../../../../koebe-quarter-theorem.md).

Suppose $G$ is [univalent](../../../../../univalent-function.md) on $|\zeta|>1$ and has a [Laurent series](../../../../../laurent-series.md)

$$
G(\zeta)=\zeta+b_0+\sum_{n=1}^{\infty}b_n\zeta^{-n}.
$$

For $R>1$, the image of $Re^{it}$, $0\le t\le2\pi$, is a regular simple closed curve. By the [Jordan curve theorem](../../../../../jordan-curve-theorem.md) the curve has one bounded and one unbounded complementary component. The image of $|\zeta|>R$ lies in the unbounded component, since it is connected, avoids the curve by injectivity and contains points near infinity. It fills that component: any finite boundary limit of the image has preimages bounded by $G(\zeta)/\zeta\to1$, and a convergent preimage subsequence must land on $|\zeta|=R$ or else give an interior image point. Thus no boundary of the image lies inside that complementary component. The curve is positively oriented about its bounded interior, since the exterior is on the right of $Re^{it}$ and a holomorphic map with nonzero [derivative](../../../../../derivative.md) preserves orientation. Green's formula gives its enclosed area as

$$
A_R=\frac1{2i}\int_0^{2\pi}\overline{G(Re^{it})}\,\frac{d}{dt}G(Re^{it})\,dt
=\pi\left(R^2-\sum_{n=1}^{\infty}n|b_n|^2R^{-2n}\right).
$$

For completeness, the positive [Fourier mode](../../../../../fourier-mode.md) is $Re^{it}$ and the negative modes are $b_nR^{-n}e^{-int}$. On multiplying by the conjugate series and integrating, all unequal-frequency products integrate to zero by [Fourier orthogonality](../../../../../fourier-orthogonality.md). The equal-frequency products give $iR^2$ and $-in|b_n|^2R^{-2n}$, respectively; the constant term gives zero. The [Laurent series](../../../../../laurent-series.md) and its differentiated series converge uniformly on the [circle](../../../../../circle.md), since $R>1$, so these operations are justified. Nonnegativity of $A_R$ yields $\sum n|b_n|^2R^{-2n}\le R^2$. Letting $R\downarrow1$, or first doing so for every finite partial sum, gives

$$
\boxed{\sum_{n=1}^{\infty}n|b_n|^2\le1.}
$$

No regularity of the map on the unit [circle](../../../../../circle.md) has been assumed.

Now let $f(z)=z+a_2z^2+\cdots$ be a [normalized univalent function](../../../../../normalized-univalent-function.md). Its only zero is at zero, so $f(z)/z$, extended there by the value one, is holomorphic and nowhere zero. On the [simply connected](../../../../../simply-connected-space.md) disc it has a [holomorphic square root](../../../../../holomorphic-square-root.md) with value one at zero. Its [odd square-root transform](../../../../../odd-square-root-transform-of-a-normalized-univalent-function.md) is

$$
h(z)=z\sqrt{\frac{f(z^2)}{z^2}}=z+\frac{a_2}{2}z^3+\cdots.
$$

This is an [odd function](../../../../../odd-function.md) which is holomorphic and normalized. It is also [univalent](../../../../../univalent-function.md): $h(z)=h(w)$ gives $f(z^2)=f(w^2)$ and hence $z=\pm w$. If $z=-w$, oddness gives $h(z)=-h(z)$, so $h(z)=0$, forcing $z=w=0$. Thus $G(\zeta)=1/h(1/\zeta)$ is [univalent](../../../../../univalent-function.md) on the exterior disc, with expansion

$$
G(\zeta)=\zeta-\frac{a_2}{2}\zeta^{-1}+\cdots.
$$

Applying the area bound to its first negative coefficient proves the [second coefficient bound for normalized univalent functions](../../../../../second-coefficient-bound-for-normalized-univalent-functions.md), **$|a_2|\le2$**.

Let $w_0$ be any point omitted by $f$. It is nonzero. Postcomposition with a [Möbius map](../../../../../mobius-transformation.md) gives another [normalized univalent function](../../../../../normalized-univalent-function.md)

$$
f_{w_0}(z)=\frac{f(z)}{1-f(z)/w_0}
=z+\left(a_2+\frac1{w_0}\right)z^2+\cdots,
$$

whose denominator does not vanish. Applying the second coefficient bound both to $f$ and to $f_{w_0}$ gives

$$
\frac1{|w_0|}\le\left|a_2+\frac1{w_0}\right|+|a_2|\le4.
$$

Every omitted point therefore has modulus at least $1/4$, proving

$$
\boxed{\{w:|w|<1/4\}\subset f(\mathbb D).}
$$

This establishes the [Koebe quarter theorem](../../../../../koebe-quarter-theorem.md) from the allowed area formula.

Sharpness is witnessed by the [Koebe function](../../../../../koebe-function.md) $k(z)=z/(1-z)^2$. It has the required value and [derivative](../../../../../derivative.md) at zero. The equality $k(z)=k(w)$ simplifies to $(z-w)(1-zw)=0$, and $|zw|<1$ makes it [injective](../../../../../injective-function.md). Moreover,

$$
k(z)+\frac14=\frac{(1+z)^2}{4(1-z)^2}\ne0\qquad(|z|<1).
$$

Thus $-1/4$ is omitted, so **no larger universal radius is possible**. In fact $4k(z)+1=((1+z)/(1-z))^2$ shows its image is the plane slit along $(-\infty,-1/4]$.

Without univalence take a real $\lambda>4$ and

$$
\boxed{f_\lambda(z)=\frac{e^{\lambda z}-1}{\lambda}.}
$$

It is [entire](../../../../../entire-function.md), with $f_\lambda(0)=0$ and $f_\lambda'(0)=1$, but it omits $-1/\lambda$, a point of modulus less than $1/4$, since the exponential never vanishes. It is genuinely not [univalent](../../../../../univalent-function.md) on the disc: the distinct points $\pm\pi i/\lambda$ lie there and both give exponential value $-1$. Even its [derivative](../../../../../derivative.md) never vanishes, illustrating why local conformality alone does not give the quarter-disc inclusion.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 9](../../paper-9-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
