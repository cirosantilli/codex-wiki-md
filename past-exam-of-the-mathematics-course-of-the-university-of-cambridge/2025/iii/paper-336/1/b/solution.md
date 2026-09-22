<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Write $w=z-1=X+iY$. The phase and its derivative are

$$
\phi=w^3+3w,
\qquad
\phi'=3(w^2+1),
$$

so the [saddle points](../../../../../../saddle-point.md) are

$$
\boxed{z_+=1+i,qquad z_-=1-i,}
$$

with $\phi(z_+)=2i$ and $\phi(z_-)=-2i$. The contour geometry can be drawn from

$$
\operatorname{Re}\phi=X(X^2-3Y^2+3),
\qquad
\operatorname{Im}\phi=Y(3X^2-Y^2+3).
$$

The stationary-phase level $\operatorname{Re}\phi=0$ consists of $X=0$ and $X^2-3Y^2+3=0$, meeting at the saddles. The steepest curves through $z_\pm$ are the levels $\operatorname{Im}\phi=\pm2$. Far away, sectors with $\cos(3\arg w)>0$ are exponential hills and those with $\cos(3\arg w)<0$ are valleys.

The stated contour deforms through the upper saddle. If $z=z_++s$, then

$$
\phi(z)=2i+3is^2+s^3.
$$

The descent tangent has $s=e^{i\pi/4}t$, because $3is^2=-3t^2$. The [simple-saddle contribution in steepest descent](../../../../../../simple-saddle-contribution-in-steepest-descent.md) is therefore

$$
f(\lambda)\sim e^{2i\lambda}e^{i\pi/4}
\int_{-\infty}^{\infty}e^{-3\lambda t^2}dt
=\boxed{\sqrt{\frac\pi{3\lambda}}e^{i\pi/4+2i\lambda}.}
$$

When the contour begins at $z=1$, deform it first from the endpoint into the decaying negative-real direction and then onto the same upper-saddle descent path. Near the endpoint, $s=z-1$ and $\phi=3s+O(s^3)$, so the [endpoint contribution in steepest descent](../../../../../../endpoint-contribution-in-steepest-descent.md) is

$$
\int_0^{-\infty}e^{3\lambda s}ds=-\frac1{3\lambda}.
$$

Adding the saddle and endpoint pieces gives

$$
\boxed{f(\lambda)\sim
\sqrt{\frac\pi{3\lambda}}e^{i\pi/4+2i\lambda}
-\frac1{3\lambda}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 336](../../../paper-336-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
