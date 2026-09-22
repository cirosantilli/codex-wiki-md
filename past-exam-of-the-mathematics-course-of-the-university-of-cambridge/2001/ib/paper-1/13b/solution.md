<h1 id="13b/solution">Solution</h1>

↑ **Parent:** [13B](../13b.md)

Project from the north pole $N=(0,0,1)$ onto the equatorial plane, identifying that plane with the [complex plane](../../../../../complex-plane.md). The line from $N$ to $P=(X,Y,Z)$ meets the plane in

$$
\boxed{\phi(P)=\frac{X+iY}{1-Z}},\qquad \phi(N)=\infty.
$$

This is [stereographic projection](../../../../../stereographic-projection.md). Its inverse is

$$
P(u)=\frac1{1+|u|^2}\bigl(2\operatorname{Re}u,2\operatorname{Im}u,|u|^2-1\bigr).
$$

Rotation through $\theta$ about the $z$-axis changes $X+iY$ to $e^{i\theta}(X+iY)$ and preserves $Z$, so it becomes the [Möbius transformation](../../../../../mobius-transformation.md) $u\mapsto e^{i\theta}u$.

Let $B$ be the rotation [matrix](../../../../../matrix.md) supplied in the question. It sends the $z$-axis to the $x$-axis, and therefore $R_x(\theta)=BR_z(\theta)B^{-1}$. If $b=\phi B\phi^{-1}$ is its given [Möbius transformation](../../../../../mobius-transformation.md), then

$$
\phi R_x(\theta)\phi^{-1}=b\circ(u\mapsto e^{i\theta}u)\circ b^{-1},
$$

which is again a [Möbius transformation](../../../../../mobius-transformation.md). Such $z$- and $x$-axis rotations can send any chosen point of the sphere to the south pole: first rotate its horizontal projection onto the $y$-axis, then rotate in the $yz$-plane. This supplies the rotations needed below.

The [antipodal stereographic coordinate relation](../../../../../antipodal-stereographic-coordinate-relation.md) is $\phi(-P)=-1/\overline{\phi(P)}$, as follows immediately from the inverse formula. Fix the [cross-ratio](../../../../../cross-ratio.md) convention

$$
[a,b;c,d]=\frac{(a-c)(b-d)}{(a-d)(b-c)}.
$$

We claim the required ordering is

$$
\boxed{\left[u,-\frac1{\bar u};v,-\frac1{\bar v}\right]=-\tan^2(d/2)}.
$$

For the [antipodal cross-ratio and spherical distance](../../../../../antipodal-cross-ratio-and-spherical-distance.md) identity, rotate $P$ to the south pole. Its coordinate becomes zero and its antipode becomes infinity. A point at angular [spherical distance](../../../../../great-circle-distance.md) $d$ from the south pole has vertical coordinate $-\cos d$ and horizontal magnitude $\sin d$, so its new projected coordinate $v'$ has modulus $\sin d/(1+\cos d)=\tan(d/2)$. By [Möbius invariance of the cross-ratio](../../../../../mobius-invariance-of-the-cross-ratio.md), the displayed expression equals

$$
[0,\infty;v',-1/\bar v']=\frac{-v'}{1/\bar v'}=-|v'|^2=-\tan^2(d/2).
$$

For finite nonsingular coordinates the same ratio is $-|u-v|^2/|1+u\bar v|^2$. Zero or infinite antipodal coordinates are interpreted by limits. When $Q=-P$, $d=\pi$ and the ratio has the extended value infinity; the finite real formula applies for $0<d<\pi$.

## ↑ Ancestors (10)

1. [13B](../13b.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
