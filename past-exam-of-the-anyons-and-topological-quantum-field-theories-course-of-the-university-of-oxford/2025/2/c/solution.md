<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $B^{ab}_c$ denote the split-fuse diagram with a charge-$c$ edge joining the lower fusion vertex to the upper splitting vertex, and outer strands $a,b$. Completeness in the [isotopy normalization of anyon diagrams](../../../../isotopy-normalization-of-anyon-diagrams.md) reads

$$
1_{a\otimes b}=\sum_c\sqrt{\frac{d_c}{d_ad_b}}\,B^{ab}_c.
$$

Resolve the two strands inside the encircling [normalized Kirby color](../../../../normalized-kirby-color.md) loop in this way. Move that loop onto the intermediate charge-$c$ edge. The [Kirby killing property](../../../../kirby-killing-property.md) multiplies it by $\mathcal D\delta_{c1}$, leaving

$$
K_\Omega(a,b)=\mathcal D\sqrt{\frac{d_1}{d_ad_b}}\,B^{ab}_1.
$$

The [vacuum anyon](../../../../vacuum-anyon.md) channel is allowed only for $b=\bar a$, and then $d_b=d_a$ and $d_1=1$. Erasing the vacuum edge turns $B^{a\bar a}_1$ into the cup-cap diagram $E_a$, which connects the incoming pair by a cap and the outgoing pair by a cup. Thus the requested [two-strand Kirby projector](../../../../two-strand-kirby-projector.md) is

$$
\boxed{K_\Omega(a,b)=\delta_{b,\bar a}\frac{\mathcal D}{d_a}\,E_a=\mathcal D P^{ab}_1.}
$$

Here $P^{a\bar a}_1=E_a/d_a$ is the [orthogonal projection](../../../../orthogonal-projection.md) onto total [vacuum anyon](../../../../vacuum-anyon.md) charge; for $b\ne\bar a$ it is zero. Both strands in the source point upwards, so the condition is $b=\bar a$, not $b=a$ unless $a$ is self-dual.

The coefficient can be checked without a convention guess: stacking two cup-cap diagrams creates one charge-$a$ loop, so $E_a^2=d_aE_a$. Consequently $(E_a/d_a)^2=E_a/d_a$, as required of an [orthogonal projection](../../../../orthogonal-projection.md). Omitting $1/d_a$ would fail this check.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2025](../../../2025-split.md)
4. [Past exam of the anyons and topological quantum field theories course of the University of Oxford](../../../split.md)
5. [Anyons and topological quantum field theories course of the University of Oxford](../../../../anyons-and-topological-quantum-field-theories-course-of-the-university-of-oxford.md)
6. [Year 4 of the mathematical and theoretical physics course of the University of Oxford](../../../../year-4-of-the-mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
7. [Mathematical and theoretical physics course of the University of Oxford](../../../../mathematical-and-theoretical-physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
