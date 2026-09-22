<h1 id="2/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Set $E=e_3$ and $\beta=3a_0(a_1-a_0)/(a_1+2a_0)$. The incident field relevant to each [sphere](../../../../../../sphere.md) is its [exciting field of a conductivity inclusion](../../../../../../exciting-field-of-a-conductivity-inclusion.md): the macroscopic field plus the regular field due to other inclusions and periodic images, excluding its own singular dipole. In the first interaction approximation write

$$
e_j^{(1)}=-\frac{\beta}{p_j}\Lambda_jE.
$$

The interior response from part (i) then gives the improved polarization

$$
P^{(1)}(x)\simeq\beta\sum_{j=1}^N\chi_{B_j}(x)\bigl(E+e_j^{(1)}\bigr).
$$

Averaging, using $\langle\chi_{B_j}\rangle=p_j$, gives

$$
\langle P^{(1)}\rangle
\simeq p\beta E+\beta\sum_jp_je_j^{(1)}
=p\beta E-\beta^2\sum_j\Lambda_jE.
$$

Therefore the [dipole interaction correction to effective conductivity](../../../../../../dipole-interaction-correction-to-effective-conductivity.md) is

$$
\boxed{
a^*\simeq a_0I+p\beta I-\beta^2\sum_{j=1}^N\Lambda_j.
}
$$

The factors $p_j$ cancel against the denominator in the given field correction. [Linearity](../../../../../../linearity.md) permits repeating the calculation for three independent incident [gradients](../../../../../../gradient.md), recovering the [tensor](../../../../../../tensor.md) rather than just its action on $e_3$. This is a second-reflection estimate; further dipole reflections and higher multipoles have been omitted.

A literal pointwise reading of the field printed “on the surface” needs qualification. Even the isolated-sphere solution in part (i) has, on a concentric [sphere](../../../../../../sphere.md) of radius $R$,

$$
e_{\mathrm{self}}(Rn)
=-\frac{r_1^3(a_1-a_0)}{(a_1+2a_0)R^3}
\bigl(I-3n\otimes n\bigr)E.
$$

For $E=e_3$, its values at $n=e_3$ and $n=e_1$ are respectively $2kr_1^3E/R^3$ and $-kr_1^3E/R^3$, where $k=(a_1-a_0)/(a_1+2a_0)$. They differ whenever there is nonzero contrast. Thus a single constant [matrix](../../../../../../matrix.md) cannot give the total pointwise field everywhere on that [sphere](../../../../../../sphere.md).

The consistent local-field interpretation is a [spherical average](../../../../../../spherical-average.md), or equivalently the regular exciting field at the centre. Indeed $\langle n\otimes n\rangle_{S}=I/3$, so the angular mean of the self-dipole is zero. The other-inclusion field is [harmonic](../../../../../../harmonic-function.md) inside the surrounding [sphere](../../../../../../sphere.md), and the [mean value property](../../../../../../mean-value-property-for-harmonic-functions.md) gives its central value. With $\Lambda_j$ encoding this average regular correction, the calculation above is justified. If “on the surface” is instead insisted upon as a constant total pointwise field, that premise is false and the isolated-sphere values above are a counterexample. The distinction between dipole fields and local exciting fields is also treated in sections 10.2–10.3 of [https://www.math.utah.edu/~milton/TheoryCompositesNOPRINT.pdf](https://www.math.utah.edu/~milton/TheoryCompositesNOPRINT.pdf) .

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [2](../../2.md)
3. [Paper 80](../../../paper-80-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
