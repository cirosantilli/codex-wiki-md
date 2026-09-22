<h1 id="17f/solution">Solution</h1>

↑ **Parent:** [17F](../17f.md)

[Jordan's lemma](../../../../../jordan-s-lemma.md) states that, for $b>0$, if $g(z)\to0$ uniformly on large upper semicircles, then $\int g(z)e^{ibz}\,dz\to0$ on those arcs. Indeed its absolute value is at most $R\max|g|\int_0^\pi e^{-bR\sin\theta}\,d\theta\le(\pi/b)\max|g|$. For negative $b$, use lower semicircles. The corresponding exponential-decay estimates can also be used on rectangular closures.

First take $a>0$ and $0<\varepsilon<a$, and define

$$
F(z)=\frac{z\sin(xz)}{(a^2+z^2)\sin(\pi z)}.
$$

Use finite strip rectangles with vertical sides at $\pm R$, $R=N+1/2$, then let $N\to\infty$. Their orientation is positive. At a nonzero integer, the [residue](../../../../../residue.md) is

$$
\operatorname{Res}_{z=n}F=\frac{(-1)^n n\sin(nx)}{\pi(a^2+n^2)}.
$$

The origin is removable when $a\ne0$ and contributes zero. The short vertical-side integrals tend to zero since $|\sin\pi(\pm R+iy)|=\cosh(\pi y)$ and $F=O(R^{-1})$ there. The [residue theorem](../../../../../residue-theorem.md) therefore gives the first evaluation,

$$
I=2i\sum_{n=-\infty}^{\infty}(-1)^n\frac{n\sin(nx)}{a^2+n^2}.
$$

The sum is understood as the limit of symmetric partial sums. It converges for $|x|<\pi$ by the [Dirichlet test](../../../../../dirichlet-test.md): the oscillatory partial sums are bounded, and $n/(a^2+n^2)$ decreases eventually to zero.

For the second evaluation, close the top line outward into the upper half-plane and the bottom line outward into the lower half-plane. Because of the strip orientations, both outward closures are clockwise. The upper region contains only the [pole](../../../../../pole.md) $ia$, and the lower one only $-ia$. Their [residues](../../../../../residue.md) are

$$
\operatorname{Res}_{ia}F=\frac{\sin(iax)}{2\sin(i\pi a)}
=\frac{\sinh(ax)}{2\sinh(\pi a)},\qquad
\operatorname{Res}_{-ia}F=\frac{\sinh(ax)}{2\sinh(\pi a)}.
$$

To justify discarding the added boundaries, use rectangles with far vertical sides at $\pm(N+1/2)$ and outer horizontal sides at imaginary height $\pm R$. The numerator grows at most like $e^{|x||\operatorname{Im}z|}$, while $1/\sin\pi z$ decays like $e^{-\pi|\operatorname{Im}z|}$. Thus the horizontal integral tends exponentially to zero, and the vertical integrals are bounded by a constant times $R^{-1}\int_\varepsilon^R e^{-(\pi-|x|)y}\,dy\to0$. The strict condition $|x|<\pi$ is essential. The clockwise [residue](../../../../../residue.md) calculation gives

$$
I=-2\pi i\left(\operatorname{Res}_{ia}F+\operatorname{Res}_{-ia}F\right)
=-2\pi i\frac{\sinh(ax)}{\sinh(\pi a)}.
$$

Equating the two evaluations proves the [alternating sine series with a quadratic denominator](../../../../../alternating-sine-series-with-a-quadratic-denominator.md):

$$
\boxed{\sum_{n=-\infty}^{\infty}(-1)^n\frac{n\sin(nx)}{a^2+n^2}
=-\pi\frac{\sinh(ax)}{\sinh(\pi a)},\qquad |x|<\pi.}
$$

Both sides are even functions of $a$, so this proves the result for every nonzero real $a$. At $a=0$ the displayed zero-index summand and right-hand ratio are literally undefined; under their natural [continuous](../../../../../continuous-function.md) extension, set that summand to zero and take the right-hand limit $-x$. This limit may be passed through the nonzero-index sum, since its difference from the $a=0$ sum is bounded by $2a^2\sum_{n\ge1}n^{-3}$. Thus the intended limiting identity at zero is $2\sum_{n\ge1}(-1)^n\sin(nx)/n=-x$. The separate contour evaluation above assumes distinct off-axis [poles](../../../../../pole.md) and should not be applied unchanged after they coalesce at the origin.

## ↑ Ancestors (10)

1. [17F](../17f.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
