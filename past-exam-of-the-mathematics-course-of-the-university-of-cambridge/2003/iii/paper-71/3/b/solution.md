<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The compressive tip [force](../../../../../../force.md) is limited by [Euler buckling of an elastic filament](../../../../../../euler-buckling-of-an-elastic-filament.md). With unsupported length $\ell$ and [filament bending modulus](../../../../../../filament-bending-modulus.md) $B=EI$,

$$
\boxed{F_c\sim\frac B{\ell^2}\sim\frac{Er^4}{\ell^2}.}
$$

For a hollow [microtubule](../../../../../../microtubule.md), use $I=\pi(r_o^4-r_i^4)/4$ rather than the solid-cylinder value. For a clamped seed and a moment-free tip free to slide along the wall, linearized angle balance is $B\theta''+F\theta=0$, with $\theta(0)=0$ and $\theta'(\ell)=0$. Its first nonzero solution has $\sqrt{F/B}\,\ell=\pi/2$, hence $F_c=\pi^2B/(4\ell^2)$. A different tip constraint changes this coefficient.

Increasing the unsupported length decreases that threshold. For growth against a wall at fixed projected gap $d$, [polymerization-driven cantilever postbuckling](../../../../../../polymerization-driven-cantilever-postbuckling.md) gives a more direct quantitative statement. The inextensible elastica obeys $B\theta''+F\sin\theta=0$. Multiplying by $\theta'$ and using the zero tip moment gives

$$
\frac B2(\theta')^2=F(\cos\theta-\cos\theta_t).
$$

Put $k=\sin(\theta_t/2)$ and substitute $\sin(\theta/2)=k\sin\phi$. Integrating arc length and its horizontal projection gives

$$
\ell=\sqrt{B/F}\,K(k),\qquad d=\sqrt{B/F}\,[2E(k)-K(k)],
$$

where the complete [elliptic integrals](../../../../../../elliptic-integral.md) are $K(k)=\int_0^{\pi/2}(1-k^2\sin^2\phi)^{-1/2}d\phi$ and $E(k)=\int_0^{\pi/2}(1-k^2\sin^2\phi)^{1/2}d\phi$. Using $K=(\pi/2)(1+k^2/4+\cdots)$ and $E=(\pi/2)(1-k^2/4+\cdots)$ gives $\ell/d=1+k^2+O(k^4)$, and therefore

$$
\boxed{F=\frac{\pi^2B}{4d^2}\left[1-\frac32\frac{\ell-d}{d}+O\left(\frac{(\ell-d)^2}{d^2}\right)\right].}
$$

Thus the initial postbuckling [force](../../../../../../force.md) decreases as more contour is inserted. This result describes the weakly buckled branch before overhang, further wall contact, or altered tip constraints invalidate the model. It is a mechanical [force](../../../../../../force.md) law; a chemical [force](../../../../../../force.md) limit from [polymerization](../../../../../../polymerization.md) can impose a smaller [force](../../../../../../force.md).

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 71](../../../paper-71-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
