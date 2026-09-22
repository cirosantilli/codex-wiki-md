<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

A point $x$ of a set $S$ is an [extreme point](../../../../../../extreme-point.md) if $x=(1-t)y+tz$, with $y,z\in S$ and $0<t<1$, forces $y=z=x$. For a [convex set](../../../../../../convex-set.md) it is enough to test midpoint decompositions: a nontrivial segment containing $x$ in its interior contains a smaller segment with midpoint $x$. The nonempty convex set $\mathbb R^2$ has no [extreme points](../../../../../../extreme-point.md), since every $x$ is the midpoint of $x+e_1$ and $x-e_1$.

For the real [l-infinity sequence space](../../../../../../l-infinity-sequence-space.md), a vector in the closed [unit ball](../../../../../../unit-ball.md) is extreme precisely when every coordinate is $1$ or $-1$. If $|x_j|<1$ for some $j$, choose $0<\delta\le1-|x_j|$. The distinct vectors $x\pm\delta e_j$ remain in the unit ball and have midpoint $x$, so $x$ is not extreme. Conversely suppose all coordinates have modulus one and $x=(y+z)/2$, with $\|y\|_\infty,\|z\|_\infty\le1$. In each real interval $[-1,1]$, an endpoint can be a midpoint only if both entries equal that endpoint. Thus $y_j=z_j=x_j$ for every $j$ and $y=z=x$. Therefore

$$
\boxed{\operatorname{ext}B_{\ell^\infty}=\{x:x_j\in\{-1,1\}\text{ for every }j\}.}
$$

For the real [absolutely summable sequence space](../../../../../../absolutely-summable-sequence-space.md), any point with $\|x\|_1<1$ is nonextreme: choose a nonzero coordinate perturbation of norm less than $1-\|x\|_1$. If $\|x\|_1=1$ and two coordinates $x_j,x_k$ are nonzero, take $0<\delta<\min(|x_j|,|x_k|)$ and put

$$
h=\delta\bigl(\operatorname{sgn}(x_j)e_j-\operatorname{sgn}(x_k)e_k\bigr).
$$

Both perturbations preserve the signs of those two coordinates. One adds $\delta$ to one absolute value and subtracts it from the other, so $\|x+h\|_1=\|x-h\|_1=1$. Hence such an $x$ is not extreme. The only remaining candidates are $\pm e_j$. If $e_j=(y+z)/2$ with $\|y\|_1,\|z\|_1\le1$, its $j$th coordinate forces $y_j=z_j=1$. That consumes the entire norm allowance, forcing all other coordinates to vanish. The argument for $-e_j$ is identical. Thus

$$
\boxed{\operatorname{ext}B_{\ell^1}=\{e_j,-e_j:j\ge1\}.}
$$

For the real [l2 sequence space](../../../../../../l2-sequence-space.md), interior points of the unit ball again permit sufficiently small opposite perturbations and are not extreme. If $\|x\|_2=1$ and $x=(y+z)/2$, write $y=x+h$, $z=x-h$. The [parallelogram law](../../../../../../parallelogram-law.md) gives

$$
\frac{\|y\|_2^2+\|z\|_2^2}{2}=\|x\|_2^2+\|h\|_2^2=1+\|h\|_2^2.
$$

The left side is at most one, so $h=0$ and $y=z=x$. Consequently

$$
\boxed{\operatorname{ext}B_{\ell^2}=\{x:\|x\|_2=1\}.}
$$

These are the [extreme points of real sequence-space unit balls](../../../../../../extreme-points-of-real-sequence-space-unit-balls.md): signs in $\ell^\infty$, coordinate spikes in $\ell^1$, and the whole sphere in $\ell^2$. The restriction to real scalars matters for the first description; the complex supremum ball has arbitrary unit-modulus coordinates instead.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 8](../../../paper-8-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
