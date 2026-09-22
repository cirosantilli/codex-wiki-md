<h1 id="14d/solution">Solution</h1>

↑ **Parent:** [14D](../14d.md)

Since

$$
\nabla\cdot(\phi\nabla\psi-\psi\nabla\phi)=\phi\nabla^2\psi-\psi\nabla^2\phi,
$$

the divergence theorem proves Green's second identity.

If $x_0=(x_0,y_0,z_0)$ and $x_0^*=(x_0,y_0,-z_0)$, the image solution is

$$
\psi(x)=-\frac1{4\pi}\left(\frac1{|x-x_0|}-\frac1{|x-x_0^*|}\right).
$$

It vanishes on the plane and has the required unit delta source.

Green's identity yields the Poisson-kernel [integral](../../../../../integral.md)

$$
\phi(x_0,y_0,z_0)=\frac1{2\pi}\iint_{x^2+y^2<1}
\frac{z_0\,dx\,dy}{[(x-x_0)^2+(y-y_0)^2+z_0^2]^{3/2}}.
$$

On the axis this becomes

$$
\boxed{\phi(0,0,z)=\int_0^1\frac{zr\,dr}{(r^2+z^2)^{3/2}}
=1-\frac z{\sqrt{1+z^2}}.}
$$

## ↑ Ancestors (10)

1. [14D](../14d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2025](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
