<h1 id="1/i/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Put $\phi=(U-c)F$. The [Rayleigh equation for inviscid shear flow](../../../../../../../rayleigh-equation-for-inviscid-shear-flow.md) becomes

$$
[(U-c)^2F']'-\alpha^2(U-c)^2F=0.
$$

Multiplication by $F^*$ and integration gives

$$
\int_0^1(U-c)^2Q\,dz=0,
\qquad
Q=|F'|^2+\alpha^2|F|^2\geq0.
$$

For $c_i>0$, its real and imaginary parts imply

$$
c_r=\frac{\int UQ\,dz}{\int Q\,dz},
\qquad
c_i^2=\frac{\int(U-c_r)^2Q\,dz}{\int Q\,dz}.
$$

Thus $c_r$ is a weighted mean of $U$ and $c_i^2$ is its weighted [variance](../../../../../../../variance-split.md). If $U_-\leq U\leq U_+$, the sharp bounded-variable variance estimate gives

$$
c_i^2\leq(U_+-c_r)(c_r-U_-).
$$

Completing the square proves [Howard's semicircle theorem](../../../../../../../howard-s-semicircle-theorem.md):

$$
\boxed{
\left(c_r-\frac{U_++U_-}{2}\right)^2+c_i^2
\leq\left(\frac{U_+-U_-}{2}\right)^2}.
$$

## ↑ Ancestors (12)

1. [B](../b.md)
2. [I](../../i.md)
3. [1](../../../1.md)
4. [Paper 331](../../../../paper-331-split.md)
5. [Iii](../../../../split.md)
6. [2023](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
