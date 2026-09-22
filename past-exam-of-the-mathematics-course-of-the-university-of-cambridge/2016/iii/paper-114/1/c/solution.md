<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The standard [CW complex](../../../../../../cw-complex.md) structure on [Real projective space](../../../../../../real-projective-space.md) has one cell in each dimension from zero to three. Its integral cellular boundary is multiplication by $2$ in even positive degrees and zero in odd degrees. Thus the integral [cellular cochain complex](../../../../../../cellular-cochain-complex.md) for $\mathbb{RP}^3$ is

$$
\mathbb Z\xrightarrow{\,0\,}\mathbb Z\xrightarrow{\,2\,}\mathbb Z\xrightarrow{\,0\,}\mathbb Z
$$

in degrees $0,1,2,3$. With coefficients $\mathbb F_2$, all its differentials vanish, so every one of these four [cohomology groups](../../../../../../cohomology-group.md) is one-dimensional.

The lift-and-divide construction of the [Bockstein homomorphism](../../../../../../bockstein-homomorphism.md) turns the integral differential $2$ into $1$ modulo $2$. Therefore $\beta:H^1\to H^2$ is an isomorphism, while the maps from degrees $0,2,3$ are zero. The [Bockstein cohomology](../../../../../../bockstein-cohomology.md) is consequently

$$
\boxed{H\beta^q(\mathbb{RP}^3;2)=\begin{cases}\mathbb F_2,&q=0,3,\\0,&\text{otherwise}.\end{cases}}
$$

For comparison, in the [mod-two cohomology ring of real projective space](../../../../../../mod-two-cohomology-ring-of-real-projective-space.md) $\mathbb F_2[t]/(t^4)$, $|t|=1$, this says $\beta(t)=t^2$, $\beta(t^2)=0$ and $\beta(t^3)=0$. The last two formulas also follow from the [Bockstein derivation rule](../../../../../../bockstein-derivation-rule.md) and the truncation $t^4=0$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 114](../../../paper-114-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
