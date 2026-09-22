<h1 id="4/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $r=|\mathbf x|$, $\theta=\mathbf x/r$, and choose $R$ so that the sphere $r=R$ strictly encloses the scatterer. Normalize the [spherical harmonics](../../../../../../../spherical-harmonic.md) to be an [orthonormal basis](../../../../../../../orthonormal-basis.md) of $L^2(S^2)$, with surface measure on the unit sphere. The outgoing [spherical Hankel function](../../../../../../../spherical-hankel-function.md) is denoted here by $h_n^{(1)}$, corresponding to the printed $H_n^{(1)}$. For fixed $n$, its large-argument behavior is

$$
h_n^{(1)}(kr)=(-i)^{n+1}\frac{e^{ikr}}{kr}\bigl(1+O(r^{-1})\bigr).
$$

Consequently the coefficient of $Y_n^m$ in the outgoing expansion is asymptotic to $a_n^m e^{ikr}/r$: the factors satisfy $i^{n+1}(-i)^{n+1}=1$. With the [far-field pattern](../../../../../../../far-field-pattern.md) defined by $u_s(r\theta)=e^{ikr}u_\infty(\theta)/r+O(r^{-2})$, we obtain

$$
\boxed{u_\infty(\theta)=\sum_{n=0}^{\infty}\sum_{m=-n}^{n}a_n^mY_n^m(\theta).}
$$

One can first project onto each [spherical harmonic](../../../../../../../spherical-harmonic.md) and then take the large-$r$ limit. This avoids assuming that the fixed-order asymptotic is uniform in $n$. The [Sommerfeld radiation condition](../../../../../../../sommerfeld-radiation-condition.md) selects the outgoing [spherical Hankel functions](../../../../../../../spherical-hankel-function.md) rather than their incoming counterparts.

Let $g(\theta)=u_s(R\theta)$. Its coefficients are $g_n^m=d_na_n^m$, where $d_n=ki^{n+1}h_n^{(1)}(kR)$. Since the field is smooth on a sphere outside the scatterer, $g\in L^2(S^2)$; [Parseval's identity](../../../../../../../parseval-identity.md) gives

$$
\|g\|_{L^2(S^2)}^2=k^2\sum_{n=0}^{\infty}|h_n^{(1)}(kR)|^2\sum_{m=-n}^{n}|a_n^m|^2<\infty.
$$

The required coefficient condition uses [fixed-argument growth of spherical Hankel functions](../../../../../../../fixed-argument-growth-of-spherical-hankel-functions.md), a different limit from the far-field limit. For fixed $t>0$,

$$
y_n(t)\sim-\frac{(2n-1)!!}{t^{n+1}},\qquad j_n(t)=O\!\left(\frac{t^n}{(2n+1)!!}\right),\qquad h_n^{(1)}(t)=j_n(t)+iy_n(t).
$$

For completeness, the series of the ordinary [Bessel function](../../../../../../../bessel-function.md) gives $J_{-n-1/2}(t)\sim(t/2)^{-n-1/2}/\Gamma(1/2-n)$. The identities $y_n(t)=(-1)^{n+1}\sqrt{\pi/(2t)}J_{-n-1/2}(t)$ and $\Gamma(1/2-n)=(-4)^nn!\sqrt\pi/(2n)!$ give the first formula; the corresponding positive-order series gives the estimate for $j_n$. The successive series corrections at fixed $t$ are $O(1/n)$. Applying [Stirling's approximation](../../../../../../../stirling-formula.md) to the factorial ratio yields

$$
(2n-1)!!=\frac{(2n)!}{2^nn!}\sim\sqrt2\left(\frac{2n}{e}\right)^n,\qquad
|h_n^{(1)}(t)|\sim\frac{\sqrt2}{t}\left(\frac{2n}{et}\right)^n.
$$

In particular there are positive constants giving upper and lower bounds by the last weight for all sufficiently large $n$. The finite trace [norm](../../../../../../../norm.md) is therefore equivalent to the [spherical far-field range condition](../../../../../../../spherical-far-field-range-condition.md)

$$
\boxed{\sum_{n=0}^{\infty}\left(\frac{2n}{ekR}\right)^{2n}\sum_{m=-n}^{n}|a_n^m|^2<\infty,}
$$

where the $n=0$ weight is defined to be one. The same conclusion holds at every larger sphere on which the outgoing field is defined.

The printed comparison with $\infty$ must mean **a finite sum**: a literal non-strict inequality allows a divergent sum. Also, the supplied one-sided big-$O$ bound alone does not imply this necessary condition from a finite trace [norm](../../../../../../../norm.md); a lower bound is needed in that direction. The two-sided asymptotic above supplies it. Conversely, its upper bound makes the weighted condition sufficient for an $L^2$ trace at the chosen sphere. This is a condition on exterior-field continuation, not a sufficient condition that the coefficients come from a particular Dirichlet obstacle.

## ↑ Ancestors (12)

1. [I](../i.md)
2. [B](../../b.md)
3. [4](../../../4.md)
4. [Paper 80](../../../../paper-80-split.md)
5. [Iii](../../../../split.md)
6. [2007](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
