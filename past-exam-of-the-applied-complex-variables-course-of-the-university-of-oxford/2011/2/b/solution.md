<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Orient the [contour](../../../../complex-integration-contour.md) and call its left-hand side the plus side. At a smooth interior point $t$, take a local arclength parameter $\gamma(s)$ with $\gamma(0)=t$. The [Cauchy principal value](../../../../cauchy-principal-value.md) means the symmetric deletion limit

$$
\operatorname{PV}\int_\Gamma\frac{f(\zeta)}{\zeta-t}\,d\zeta
=\lim_{\varepsilon\downarrow0}\int_{\Gamma\setminus\gamma((-\varepsilon,\varepsilon))}\frac{f(\zeta)}{\zeta-t}\,d\zeta.
$$

The two local pieces are deleted with the same arclength cutoff. For a sufficiently smooth regular [contour](../../../../complex-integration-contour.md), an equal-radius deletion about $t$ gives the same limit. The point is assumed to be away from endpoints and self-intersections.

To derive the [Sokhotski–Plemelj formula](../../../../sokhotski-plemelj-theorem.md), split the [contour](../../../../complex-integration-contour.md) into a short smooth arc through $t$ and its complement. The complementary [integral](../../../../integral-split.md) has the same limit from both sides. On the short arc subtract $f(z)$ from the numerator. Because $f$ is [holomorphic](../../../../holomorphic-function-split.md) nearby, $(f(\zeta)-f(z))/(\zeta-z)$ extends continuously as $\zeta$ approaches $z$; this part also has the same limit from either side. The remaining local term is $f(z)\int d\zeta/(\zeta-z)$. Straightening the oriented tangent shows its extra contribution is $+i\pi f(t)$ from the left and $-i\pi f(t)$ from the right: on a real segment this is the direct limit of $\int_{-\delta}^{\delta}du/(u\mp i\varepsilon)$. Dividing by $2\pi i$ yields

$$
\boxed{w_\pm(t)=\pm\frac12f(t)+\frac1{2\pi i}\operatorname{PV}\int_\Gamma\frac{f(\zeta)}{\zeta-t}\,d\zeta.}
$$

In particular the jump is $w_+-w_-=f$, while the sum is the principal-value [integral](../../../../integral-split.md) divided by $\pi i$. Smooth densities on a real interval satisfy the same formulas at every interior point, by the identical subtraction step with a Hölder-[continuous](../../../../continuous-function.md) remainder.

Now put $h=w/\widetilde w$. On the interval, the sign reversal of the auxiliary [boundary values](../../../../boundary-value.md) gives

$$
h_+-h_-=\frac{w_+}{\widetilde w_+}-\frac{w_-}{\widetilde w_-}=\frac{w_++w_-}{\widetilde w_+}=\frac{G}{\widetilde w_+}.
$$

Thus the required [Cauchy transform](../../../../cauchy-transform.md) density is

$$
\boxed{F(\xi)=\frac{G(\xi)}{\widetilde w_+(\xi)}.}
$$

Whenever this density is integrable at the endpoints, taking $h=C[F]$ constructs a [function](../../../../function-split.md) with the required jump. Multiplication back gives $w_++w_-=G$. The jump of the constructed $w$ is

$$
f(x)=w_+(x)-w_-(x)=\widetilde w_+(x)(h_+(x)+h_-(x))
=\boxed{\frac{\widetilde w_+(x)}{\pi i}\operatorname{PV}\int_0^1\frac{G(\xi)}{\widetilde w_+(\xi)(\xi-x)}\,d\xi.}
$$

To conclude that this jump solves the final singular equation, one must additionally justify $w=C[f]$. This reconstruction requires endpoint and [infinity](../../../../infinity.md) conditions; the sign reversal of $\widetilde w$ alone does not ensure it. Here is a complete valid normalization. Let

$$
S(z)=\sqrt{z(z-1)},\qquad S(z)\sim z\text{ at infinity},\qquad \widetilde w(z)=\frac1{S(z)}.
$$

The branch is [holomorphic](../../../../holomorphic-function-split.md) off $[0,1]$, with $S_+(x)=i\sqrt{x(1-x)}$ and $S_-=-S_+$. If $G$ extends smoothly to $[0,1]$, the density $F=G/\widetilde w_+=i\sqrt{x(1-x)}G$ vanishes like a [square root](../../../../square-root.md) at each endpoint. Its [Cauchy transform](../../../../cauchy-transform.md) $h$ is bounded at the endpoints and is $O(z^{-1})$ at [infinity](../../../../infinity.md). Therefore $w=h/S$ is at most inverse-square-root singular at each endpoint and is $O(z^{-2})$ at [infinity](../../../../infinity.md). Its jump $f$ is integrable.

For [Cauchy reconstruction from a jump across a finite interval](../../../../cauchy-reconstruction-from-a-jump-across-a-finite-interval.md), apply the [Cauchy integral formula](../../../../cauchy-integral-formula.md) to $w$ on a large slit [contour](../../../../complex-integration-contour.md), and shrink its banks to $[0,1]$. The large circle contributes zero in the limit; each small endpoint circle contributes $O(\sqrt\varepsilon)$ and also vanishes. The two banks give the jump $f$, proving $w=C[f]$. The sum part of the [Sokhotski–Plemelj formula](../../../../sokhotski-plemelj-theorem.md) now gives

$$
\boxed{\frac1{\pi i}\operatorname{PV}\int_0^1\frac{f(\xi)}{\xi-x}\,d\xi=G(x),\qquad0<x<1.}
$$

This proves the intended [finite Hilbert transform inversion](../../../../finite-hilbert-transform-inversion.md) with admissible endpoint behavior. Adding a multiple of $1/\sqrt{x(1-x)}$ to $f$ gives a homogeneous solution; equivalently one can add a constant multiple of $1/S$ to $w$, whose [boundary](../../../../boundary-of-a-set.md) sum is zero.

The omitted normalization is a real limitation of the printed claim. To see it explicitly, choose instead $\widetilde w=S$ and $G=1$. This auxiliary [function](../../../../function-split.md) satisfies all the stated holomorphicity, nonvanishing and sign-reversal requirements. But

$$
\int_0^1\frac{d\xi}{\sqrt{\xi(1-\xi)}(\xi-z)}=-\frac\pi{S(z)},\qquad h=C[1/S_+]=\frac1{2S(z)},\qquad w=Sh=\frac12.
$$

The displayed [integral](../../../../integral-split.md) identity follows from $\xi=(1+\cos\theta)/2$ and its continuation from real $z>1$. Hence the proposed jump formula gives $f=0$, which does not solve the equation with $G=1$. The failure is the nonzero constant at [infinity](../../../../infinity.md): $w-C[f]=1/2$. Thus **the final implication is valid with suitable endpoint and decay conditions, but is false for an unrestricted auxiliary [function](../../../../function-split.md) as printed**. The valid reciprocal-square-root normalization above supplies an actual solution for $G$ smooth up to the two endpoints.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [2](../../2.md)
3. [2011](../../../2011-split.md)
4. [Past exam of the applied complex variables course of the University of Oxford](../../../split.md)
5. [Applied complex variables course of the University of Oxford](../../../../applied-complex-variables-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematics course of the University of Oxford](../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
