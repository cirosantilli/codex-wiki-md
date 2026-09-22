<h1 id="39a/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

On $r=c$, the traction $\boldsymbol\sigma\mathbf n$ exerted by the outer fluid on the inner fluid is

$$
\boldsymbol\sigma\mathbf n
=-\frac{3\mu B}{c^3}
(\boldsymbol\Omega\times\mathbf n).
$$

The inner fluid exerts the opposite traction on the outer fluid. Its couple is therefore

$$
\begin{aligned}
\mathbf G
&=-\int_{r=c}\mathbf x\times
(\boldsymbol\sigma\mathbf n)\,dS\\
&=3\mu Bc^{-2}
\int_{r=c}\mathbf n\times
(\boldsymbol\Omega\times\mathbf n)\,dS.
\end{aligned}
$$

Using

$$
\mathbf n\times(\boldsymbol\Omega\times\mathbf n)
=\boldsymbol\Omega-\mathbf n(\mathbf n\cdot\boldsymbol\Omega)
$$

and the supplied spherical integral,

$$
\int_{r=c}n_in_j\,dS
=\frac{4\pi c^2}{3}\delta_{ij},
$$

we obtain

$$
\int_{r=c}\mathbf n\times
(\boldsymbol\Omega\times\mathbf n)\,dS
=\frac{8\pi c^2}{3}\boldsymbol\Omega.
$$

Thus the radius cancels:

$$
\mathbf G=8\pi\mu B\boldsymbol\Omega
=\boxed{
\frac{8\pi\mu a^3b^3}{b^3-a^3}
\boldsymbol\Omega}.
$$

This is the [Torque in rotational Stokes flow between concentric spheres](../../../../../../../torque-in-rotational-stokes-flow-between-concentric-spheres.md).

When $a\ll b$,

$$
\mathbf G\sim8\pi\mu a^3\boldsymbol\Omega,
$$

the rotational drag torque for a sphere in an effectively unbounded fluid. If $h=b-a\ll a$, then

$$
b^3-a^3\sim3a^2h,
\qquad
a^3b^3\sim a^6,
$$

so

$$
\mathbf G\sim
\frac{8\pi\mu a^4}{3h}\boldsymbol\Omega,
$$

the inverse-gap growth expected from a thin [Couette flow](../../../../../../../couette-flow.md).

## ↑ Ancestors (12)

1. [Iv](../iv.md)
2. [B](../../b.md)
3. [39A](../../../39a.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2021](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
