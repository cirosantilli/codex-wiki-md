<h1 id="14c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

There is a branch-phase discrepancy in the printed identity. Set $K(z)=\int_{-1}^1e^t(1-t^2)^zdt$ using the positive real base. Shrink the anticlockwise loop at $1$. The outward interval carries phase $e^{-i\pi z}$ and its return phase $e^{i\pi z}$; their difference gives $-2i\sin(\pi z)\int_0^1e^t(1-t^2)^zdt$. The clockwise loop at $-1$ starts with phase $e^{i\pi z}$ and returns with $e^{-i\pi z}$, giving the same coefficient on $(-1,0)$. Small endpoint circles vanish for $\operatorname{Re}z>-1$. Thus the [branch phase in a figure-eight analytic continuation integral](../../../../../../branch-phase-in-a-figure-eight-analytic-continuation-integral.md) is

$$
\boxed{J(z)=-2i\sin(\pi z)K(z).}
$$

If the printed interval integral uses the prescribed argument $-\pi$, then $I(z)=e^{-i\pi z}K(z)$, and the corrected formula is instead

$$
\boxed{J(z)=-2i e^{i\pi z}\sin(\pi z)I(z).}
$$

For example at $z=1/2$, $K>0$, $I=-iK$ and $J=-2iK$; the printed right side without the phase would be the real number $-2K$. Interpreting its interval integrand as $(1-t^2)^z$ restores the intended identity.

On the fixed contour away from its branch points, the continued logarithm is bounded and $e^t\exp[z\log(t^2-1)]$ is entire in $z$, uniformly on compact sets. Hence $J$ is an [entire function](../../../../../../entire-function.md). Division by the sine gives a [meromorphic continuation](../../../../../../meromorphic-continuation.md) of $K$, and multiplication by $e^{-i\pi z}$ gives the continuation of the specified $I$. The only candidate singularities are integers, at most simple. All $0,1,2,\ldots$ are removable because the interval integral is already holomorphic on $\operatorname{Re}z>-1$.

The negative integers $z=-n$, $n\ge1$, are genuine [simple poles](../../../../../../simple-pole.md). At such a point the contour integrand is single-valued and

$$
J(-n)=2\pi i\left[\operatorname{Res}_{t=1}\frac{e^t}{(t^2-1)^n}-\operatorname{Res}_{t=-1}\frac{e^t}{(t^2-1)^n}\right].
$$

The first residue is $e$ times a rational number. The second is $e^{-1}$ times a nonzero rational number: expand $e^s(-2+s)^{-n}$ at $s=0$, whose degree-$n-1$ coefficient has sign $(-1)^n$ and nonzero magnitude. They cannot be equal because $e^2$ is irrational. Therefore $J(-n)\ne0$, and the simple sine zero creates a [simple pole](../../../../../../simple-pole.md). In particular $\operatorname{Res}_{z=-n}K=-J(-n)/[2\pi i(-1)^n]$.

A circle enclosing both branch points has total logarithmic change $4\pi i$, rather than zero as for the figure eight. For a circle based at $t=2$ with initial real logarithm, shrinking it leaves a connector from $1$ to $2$ as well as the two banks of the interval. Explicitly its integral is

$$
J_C(z)=2i e^{2\pi iz}\sin(\pi z)K(z)+(e^{4\pi iz}-1)\int_1^2e^t(t^2-1)^zdt.
$$

Thus it is not just a known sine factor times $K$: an additional endpoint-singular integral remains. The figure-eight contour eliminates precisely that connector term. This explains why replacing it by the large circle does not give the same direct continuation method.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [14C](../../14c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
