<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

At a surface [point](../../../../../point-geometry.md) $p$, let $\hat N$ be the outward [unit normal vector](../../../../../unit-normal.md), $\hat V$ the [unit vector](../../../../../unit-vector.md) from $p$ toward the viewer, and $\hat L$ the [unit vector](../../../../../unit-vector.md) from $p$ toward the light. The incoming propagation direction is therefore $-\hat L$. The [specular reflection](../../../../../specular-reflection.md) direction $\hat R$ points away from the surface along the ideal reflected ray.

Resolve $\hat L$ into its normal and tangential components:

$$
\hat L=(\hat N\cdot\hat L)\hat N+\bigl(\hat L-(\hat N\cdot\hat L)\hat N\bigr).
$$

Reflection of the incoming direction preserves its tangential component and reverses its normal component. Equivalently, the outgoing direction has the same normal component as $\hat L$ and the opposite tangential component, giving

$$
\boxed{\hat R=2(\hat N\cdot\hat L)\hat N-\hat L.}
$$

The [dot product](../../../../../dot-product.md) identity shows $\|\hat R\|=1$ when $\|\hat L\|=\|\hat N\|=1$.

In the [Phong reflection model](../../../../../phong-reflection-model.md), ambient lighting approximates unmodelled indirect illumination and is independent of these directions. The diffuse term models [Lambertian reflectance](../../../../../lambertian-reflectance.md) and varies as $\max(0,\hat N\cdot\hat L)$. The specular term models a highlight around $\hat R$ and varies as $\max(0,\hat R\cdot\hat V)^n$, where $n>0$ controls its sharpness. For a visible front surface, a convenient per-colour-channel equation is

$$
\boxed{I=k_a I_a+I_L\left[k_d\max(0,\hat N\cdot\hat L)+k_s\,\chi\,\max(0,\hat R\cdot\hat V)^n\right],}
$$

where $I_a$ is ambient illumination, $I_L$ is the source strength at the surface including any chosen attenuation, $k_a,k_d,k_s\geq0$ are material weights, and $\chi$ is one when $\hat N\cdot\hat L>0$ and zero otherwise. The weights can be colour-dependent. An idealized point source's incident strength decreases as inverse distance squared; the empirical equation can also use a prescribed attenuation law.

In degenerate geometric cases the effective weights switch off. A light behind or tangent to the surface contributes neither direct diffuse nor specular illumination. If $\hat R\cdot\hat V\leq0$, the specular term is zero. A viewpoint on the back side is rejected by [back-face culling](../../../../../back-face-culling.md) for a one-sided surface. A material with no highlight has $k_s=0$; with no diffuse response, $k_d=0$; without ambient illumination the ambient term vanishes. These zeros do not require renormalizing the other weights, and the empirical [Phong reflection model](../../../../../phong-reflection-model.md) does not impose a universal condition $k_a+k_d+k_s=1$. At coincident light/surface or eye/surface positions a direction cannot be normalized; such singular configurations require a separate convention, rather than substituting an undefined [unit vector](../../../../../unit-vector.md) into the formula.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Computer graphics](../../../computer-graphics-split.md)
4. [2015](../../../split.md)
5. [Past exam of the computer science course of the University of Oxford](../../../../split.md)
6. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
7. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
8. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
9. [University of Oxford](../../../../../university-of-oxford-split.md)
10. [List of universities](../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../split.md)
