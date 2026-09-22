<h1 id="2/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let the incident plane wave be

$$
\psi_i(\mathbf r)
=e^{ik_0\widehat{\mathbf r}_0\cdot\mathbf r},
$$

and define the scattering vector

$$
\mathbf q=k_0
(\widehat{\mathbf r}-\widehat{\mathbf r}_0).
$$

For $r$ much larger than the diameter of $D$, the [far-field pattern](../../../../../../far-field-pattern.md) follows from

$$
G_0(\mathbf r-\mathbf r')
\sim\frac{e^{ik_0r}}{4\pi r}
e^{-ik_0\widehat{\mathbf r}\cdot\mathbf r'}.
$$

Writing

$$
\widetilde V(\mathbf q)
=\int_DV(\mathbf r')e^{-i\mathbf q\cdot\mathbf r'}\,d^3r',
$$

the Born result is

$$
\boxed{
\psi_B(\mathbf r)
\sim e^{ik_0\widehat{\mathbf r}_0\cdot\mathbf r}
+\frac{e^{ik_0r}}{4\pi r}
\widetilde V(\mathbf q)}.
$$

The corresponding Rytov logarithmic perturbation is

$$
\phi_1(\mathbf r)
\sim a(\mathbf r)\widetilde V(\mathbf q),
\qquad
a(\mathbf r)=
\frac{e^{ik_0(r-\widehat{\mathbf r}_0\cdot\mathbf r)}}
{4\pi r}.
$$

Therefore

$$
\boxed{
\psi_R(\mathbf r)
\sim e^{ik_0\widehat{\mathbf r}_0\cdot\mathbf r}
\exp\left[a(\mathbf r)\widetilde V(\mathbf q)\right]}.
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [2](../../2.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
