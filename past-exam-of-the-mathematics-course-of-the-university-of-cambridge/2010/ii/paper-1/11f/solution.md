<h1 id="11f/solution">Solution</h1>

↑ **Parent:** [11F](../11f.md)

Inversion in a circle of center $c$ and radius $R$ is $K(z)=c+R^2/(\bar z-\bar c)$ on the extended plane. It sends infinity to $c$, so **it interchanges zero and infinity exactly when $c=0$**.

For the unit-circle inversion $J$, both $J$ and $K$ are involutions. If $KJz_0=z_0$, applying $K$ gives $Jz_0=Kz_0$. Writing $w=Jz_0$, we have $Jw=z_0$ and $Kw=z_0$, and therefore $KJw=Kz_0=w$. This proves both assertions about the [fixed points](../../../../../fixed-point.md).

We now show that one [fixed point](../../../../../fixed-point.md) is inside the disk and use it as the hyperbolic center. Rotate coordinates to make the Euclidean center $c=a\geq0$. The hypothesis is $a+R<1$. If $a=0$ the conclusion follows immediately from the radial hyperbolic distance. If $a>0$, then

$$
T(z)=a+\frac{R^2z}{1-az},\qquad
az^2-(1+a^2-R^2)z+a=0
$$

for its [fixed points](../../../../../fixed-point.md). Since $1+a^2-R^2>2a$, this quadratic has two positive roots with product one, one $p\in(0,1)$ and the other $1/p>1$.

The disk automorphism $h(z)=(z-p)/(1-pz)$ is a [Poincare disc automorphism](../../../../../poincare-disc-automorphism.md). It sends the two [fixed points](../../../../../fixed-point.md) to zero and infinity and commutes with $J$ on the extended plane. Consequently $K'=hKh^{-1}=(hTh^{-1})J$ interchanges zero and infinity. Conjugation takes circle inversion to inversion in the image circle, so the first part says that $h(\Gamma)$ is centered at zero. Its Euclidean radius is some $s<1$.

In the Poincaré disk metric, integrating the radial length element gives

$$
d_D(0,z)=\int_0^{|z|}\frac{2\,dr}{1-r^2}=2\operatorname{artanh}|z|.
$$

Since $h$ preserves distance, the original circle is exactly

$$
\boxed{\Gamma=\{z\in D:d_D(p,z)=2\operatorname{artanh}s\}.}
$$

Undoing the preliminary rotation gives the center for arbitrary complex $c$.

This identifies the [hyperbolic circle in the Poincare disc](../../../../../hyperbolic-circle-in-the-poincare-disc.md) intrinsically.

## ↑ Ancestors (10)

1. [11F](../11f.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
