<h1 id="24f/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Take the [punctured complex plane](../../../../../../punctured-complex-plane.md)

$$
D=\mathbb C^*=\mathbb C\setminus\{0\}
$$

and

$$
u(z)=\log|z|.
$$

In [polar coordinates](../../../../../../polar-coordinates.md), $u(r,\theta)=\log r$, so

$$
\Delta u=u_{rr}+\frac1r u_r+\frac1{r^2}u_{\theta\theta}
=-\frac1{r^2}+\frac1{r^2}=0.
$$

Thus $u$ is harmonic on $D$.

If $u=\operatorname{Re}f$ for a holomorphic function $f$, the calculation from part (a) would give

$$
f'(z)=u_x-iu_y=\frac1z.
$$

The integral of a derivative around a closed curve is zero, whereas the [residue theorem](../../../../../../residue-theorem.md) gives

$$
\int_{|z|=1}\frac{dz}{z}=2\pi i.
$$

This contradiction proves that no such $f$ exists. It is precisely the [log modulus has no global harmonic conjugate on the punctured plane](../../../../../../log-modulus-has-no-global-harmonic-conjugate-on-the-punctured-plane.md) obstruction.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [24F](../../24f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
