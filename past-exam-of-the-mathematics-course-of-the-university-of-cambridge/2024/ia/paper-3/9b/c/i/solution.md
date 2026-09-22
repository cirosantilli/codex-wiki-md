<h1 id="9b/c/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For a radial [function](../../../../../../../function-split.md) in three dimensions, the [radial Laplacian](../../../../../../../radial-laplacian.md) gives

$$
\nabla^2\phi=\frac1{r^2}(r^2\phi')'.
$$

Here regularity at zero selects

$$
r^2\phi'(r)=\int_0^rs^2(s-1)e^s\,ds
=e^r(r^3-4r^2+8r-8)+8.
$$

A further integration gives

$$
\phi(r)=\frac{e^r(r^2-5r+8)-8}{r}+C,
$$

whose apparent singularity is removable, with [limit](../../../../../../../limit-of-a-function.md) $3+C$ at zero. Since the nonconstant term has value $4e-8$ at $r=1$, the [boundary condition](../../../../../../../boundary-condition.md) $\phi(1)=3$ gives $C=11-4e$. Therefore

$$
\boxed{\phi(r)=
\frac{e^r(r^2-5r+8)-8}{r}+11-4e}.
$$

## ↑ Ancestors (12)

1. [I](../i.md)
2. [C](../../c.md)
3. [9B](../../../9b.md)
4. [Paper 3](../../../../paper-3-split.md)
5. [Ia](../../../../split.md)
6. [2024](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
