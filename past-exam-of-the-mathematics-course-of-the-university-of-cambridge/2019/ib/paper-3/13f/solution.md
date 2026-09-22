<h1 id="13f/solution">Solution</h1>

↑ **Parent:** [13F](../13f.md)

For a closed piecewise smooth path $\gamma$ avoiding $w$, its [winding number](../../../../../winding-number.md) is

$$
\boxed{n(\gamma,w)=\frac1{2\pi i}\int_\gamma\frac{dz}{z-w}}.
$$

A meromorphic function has a zero of order $m>0$ at $z_0$ when

$$
f(z)=(z-z_0)^m g(z),
\qquad g(z_0)\ne0,
$$

with $g$ holomorphic; it has a pole of order $m$ at $w_0$ when $(z-w_0)^mf(z)$ extends holomorphically and nonvanishingly there.

The [argument principle](../../../../../argument-principle.md) states that, if $f$ has no zero or pole on $\gamma$,

$$
\frac1{2\pi i}\int_\gamma\frac{f'(z)}{f(z)}\,dz
=\sum_a n(\gamma,a)\operatorname{ord}_a(f).
$$

For a positively oriented simple contour this is the number of enclosed zeros minus poles, counted with multiplicity. It follows from the [residue theorem](../../../../../residue-theorem.md) because the residue of $f'/f$ at a zero of order $m$ is $m$, while at a pole of order $m$ it is $-m$.

Let

$$
p(z)=z^4+10z^3+4z^2+10z+5.
$$

On the imaginary axis,

$$
p(iy)=\underbrace{(y^4-4y^2+5)}_{(y^2-2)^2+1>0}
+10iy(1-y^2).
$$

Thus $p(iy)$ always lies in the open right half-plane, has no zero there, and its continuous argument has net change zero as the imaginary-axis part of a large right-half-disc contour is traversed. On the right semicircle, $p(z)/z^4\to1$ uniformly, so the argument change tends to that of $z^4$, namely $4\pi$. The argument principle therefore gives

$$
\boxed{\frac{4\pi}{2\pi}=2}
$$

roots in the open right half-plane, counted with multiplicity.

## ↑ Ancestors (10)

1. [13F](../13f.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2019](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
