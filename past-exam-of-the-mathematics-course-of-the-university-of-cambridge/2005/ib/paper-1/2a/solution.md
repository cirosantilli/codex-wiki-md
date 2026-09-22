<h1 id="2a/solution">Solution</h1>

↑ **Parent:** [2A](../2a.md)

The image is a [ring torus](../../../../../ring-torus.md): a circle of radius $b$ is rotated about the vertical axis at distance $a$ from that axis. Put $r=\sqrt{x^2+y^2}$. Since $a>b$, every image point has $r>0$, and the image is precisely

$$
T=\{(x,y,z):(r-a)^2+z^2=b^2\}.
$$

Conversely, on this [level set](../../../../../level-set.md) the pairs $((r-a)/b,z/b)$ and $(x/r,y/r)$ are unit vectors, so choosing their angles gives a preimage.

The specified angular rectangle removes two closed circles from the [torus](../../../../../torus.md). More explicitly its image is

$$
U=T\setminus(C_u\cup C_v),\qquad
C_u=\{z=0,\ r=a+b\}\cap T,\quad
C_v=\{y=0,\ x>0\}\cap T.
$$

Here $C_u$ is the outer equatorial circle and $C_v$ is a meridian. The given openness property makes $U$ open in $T$. On $U$, the angles of $(r-a)+iz$ and $x+iy$ are uniquely chosen in $(0,2\pi)$; their continuous argument branches give the inverse $(x,y,z)\mapsto(u,v)$. Thus the restriction is a [homeomorphism](../../../../../homeomorphism.md) onto $U$, and the inverse is locally [smooth](../../../../../smooth-function.md).

For the [immersion](../../../../../immersion.md) condition, the two derivatives have [inner products](../../../../../inner-product.md)

$$
\sigma_u\cdot\sigma_u=b^2,\qquad
\sigma_v\cdot\sigma_v=(a+b\cos u)^2,\qquad
\sigma_u\cdot\sigma_v=0.
$$

They are [linearly independent](../../../../../linear-independence.md) everywhere, since $a+b\cos u\ge a-b>0$. Hence this is a smooth [embedded surface parametrization](../../../../../embedded-surface-parametrization.md).

The angular cuts do not represent singularities of the [embedded torus of revolution](../../../../../embedded-torus-of-revolution.md). To give a direct proof covering all points, define $F=(\sqrt{x^2+y^2}-a)^2+z^2-b^2$ on the open region $r>0$. On $T$,

$$
\nabla F=2\left((r-a)\frac{x}{r},(r-a)\frac{y}{r},z\right),\qquad
|\nabla F|=2b>0.
$$

The [implicit function theorem](../../../../../implicit-function-theorem.md) therefore describes $T$ near every point as a [smooth](../../../../../smooth-function.md) graph of two coordinates. **The whole torus is a smooth embedded surface.**

## ↑ Ancestors (10)

1. [2A](../2a.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
