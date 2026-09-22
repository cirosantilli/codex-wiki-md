<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $a$ denote tube cross-sectional area in this question, not a filament or sphere radius. The bacterial density is uniform across that section in this one-dimensional [Keller--Segel model](../../../../../../keller-segel-model.md), so the total bacterial number is

$$
N=a\int_{-\infty}^{\infty}B(z)\,dz.
$$

Integrating the nutrient balance $vC'=kB$ across the complete band gives

$$
v[C(+\infty)-C(-\infty)]=k\int_{-\infty}^{\infty}B(z)\,dz
=\frac{kN}{a}.
$$

Hence the [speed of a nutrient-consuming chemotactic band](../../../../../../speed-of-a-nutrient-consuming-chemotactic-band.md) is

$$
\boxed{v=\frac{Nk}{aC_\infty}.}
$$

This is a nutrient budget: the whole population consumes at rate $Nk$, while advancement of the band at speed $v$ brings fresh nutrient at rate $a v C_\infty$. The [conservation of mass](../../../../../../mass-conservation.md) equation for bacteria ensures $N$ stays constant when there is no flux at infinity and no cell birth or death.

At fixed total bacterial number, the speed grows linearly with $N$ and the per-cell consumption rate $k$, and decreases with tube area and nutrient concentration ahead. More nutrient takes longer to deplete, giving the inverse dependence on $C_\infty$. Although $D$ and $\alpha$ determine the width, skewness, peak density and admissibility of the smooth band, they do not appear in this speed when $N,k,a,C_\infty$ are fixed. This independence relies on neglecting nutrient diffusion and using the specified concentration-independent consumption law; it is not a general prediction for all [chemotaxis](../../../../../../chemotaxis.md) models. Dimensionally $Nk$ is nutrient amount per time and $aC_\infty$ nutrient amount per length, so their ratio is a velocity.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 342](../../../paper-342-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
