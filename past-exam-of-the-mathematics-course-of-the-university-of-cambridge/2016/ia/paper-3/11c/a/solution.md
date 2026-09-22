<h1 id="11c/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [product rule](../../../../../../product-rule.md) for the [divergence](../../../../../../divergence.md) gives

$$
\nabla\cdot(u\nabla v)=\nabla u\cdot\nabla v+u\nabla^2v,\qquad\nabla\cdot(v\nabla u)=\nabla v\cdot\nabla u+v\nabla^2u.
$$

Subtracting cancels the two [gradient](../../../../../../gradient.md) products. **Therefore**

$$
\boxed{\nabla\cdot(u\nabla v-v\nabla u)=u\nabla^2v-v\nabla^2u.}
$$

To obtain the requested order of terms, apply this identity with $u,v$ interchanged and use the [divergence theorem](../../../../../../divergence-theorem.md) on the spherical shell. On the outer sphere the shell's outward [unit normal](../../../../../../unit-normal.md) is $\widehat{\mathbf r}$; on the inner sphere it is $-\widehat{\mathbf r}$. Write $\partial_r=\widehat{\mathbf r}\cdot\nabla$ on both spheres. Then the resulting [Green second identity](../../../../../../green-second-identity.md) is

$$
\boxed{\int_{\rho\leq|\mathbf x|\leq r}(v\nabla^2u-u\nabla^2v)\,dV=\int_{|\mathbf x|=r}(v\partial_ru-u\partial_rv)\,dS-\int_{|\mathbf x|=\rho}(v\partial_ru-u\partial_rv)\,dS.}
$$

The minus sign records the inward radial direction of the shell's normal on its inner boundary. Thus the normal derivatives in the displayed difference are outward from each individual ball; using shell-outward normals instead would put a plus sign between the two boundary integrals.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11C](../../11c.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
