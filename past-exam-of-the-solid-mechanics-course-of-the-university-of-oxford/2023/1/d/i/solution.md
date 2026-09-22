<h1 id="1/d/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Using $a=A$ and the end-face [shear stress](../../../../../shear-stress.md) from part (c), the printed [torque](../../../../../torque.md) normalization gives

$$
M(\tau)=2\tau\int_0^A\left[\mu_1+\mu_2(3+\tau^2r^2)^n\right]r^3\,dr.
$$

The [binomial theorem](../../../../../binomial-theorem.md) expands the remaining [integral](../../../../../integral-split.md) into powers of $r$:

$$
(3+\tau^2r^2)^n
=\sum_{k=0}^n\binom nk3^{n-k}\tau^{2k}r^{2k}.
$$

Integrating each term gives an expression valid also at $\tau=0$:

$$
\boxed{M(\tau)=\frac{\mu_1A^4}{2}\tau
+\mu_2\sum_{k=0}^n\binom nk
\frac{3^{n-k}A^{2k+4}}{k+2}\tau^{2k+1}.}
$$

For example, $n=1$ gives $M=(\mu_1+3\mu_2)A^4\tau/2+\mu_2A^6\tau^3/3$. The [torque](../../../../../torque.md) is an odd [polynomial](../../../../../polynomial-split.md) in the twist per unit reference length, as expected when reversing the twist reverses the end-face [shear stress](../../../../../shear-stress.md).

For a physical end-face [torque](../../../../../torque.md) $N$, integration over the azimuth normally gives

$$
N=\int_0^{2\pi}\!\int_0^A T_{\theta z}r^2\,dr\,d\theta=2\pi M.
$$

The original PDF explicitly defines $M$ without this $2\pi$, so the boxed answer retains its convention. Since $\mathbf T$ is the [Cauchy stress tensor](../../../../../cauchy-stress-tensor.md), its shear component here is spatial $T_{\theta z}$; the printed capital $Z$ in $T_{\theta Z}$ does not require a change to a [nominal stress tensor](../../../../../nominal-stress-tensor.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [D](../../d.md)
3. [1](../../../1.md)
4. [2023](../../../../2023-split.md)
5. [Past exam of the solid mechanics course of the University of Oxford](../../../../split.md)
6. [Solid mechanics course of the University of Oxford](../../../../../solid-mechanics-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
