<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

The space is the [mapping torus](../../../../../mapping-torus.md) of the [antipodal map](../../../../../antipodal-map.md) $A:S^2\to S^2$. Its [mapping degree](../../../../../degree-of-a-continuous-mapping.md) is $(-1)^3=-1$, so transporting a fiber orientation once around the base circle reverses it. **$X$ is nonorientable.**

On integral fiber [homology](../../../../../homology-split.md), $A_*$ is the identity in degree zero and minus the identity in degree two. The [Wang sequence](../../../../../wang-sequence.md), whose relevant map is $1-A_*$, therefore gives

$$
H_0(X;\mathbb Z)=H_1(X;\mathbb Z)=\mathbb Z,\qquad H_2(X;\mathbb Z)=\mathbb Z/2,\qquad H_3(X;\mathbb Z)=0.
$$

The [universal coefficient theorem for cohomology](../../../../../universal-coefficient-theorem-for-cohomology.md) shifts the torsion contribution into degree three, because $\operatorname{Ext}_{\mathbb Z}(\mathbb Z/2,\mathbb Z)=\mathbb Z/2$. Hence

$$
\boxed{H^q(X;\mathbb Z)=\begin{cases}\mathbb Z,&q=0,1,\\\mathbb Z/2,&q=3,\\0,&\text{otherwise}.\end{cases}}
$$

Let $t\in H^1(X;\mathbb Z)$ be pulled back from the base circle, and $u$ the nonzero degree-three class. The square of the circle class vanishes, so $t^2=0$. All other products of positive-degree classes land above dimension three and vanish. This gives the [cohomology ring of the antipodal two-sphere mapping torus](../../../../../cohomology-ring-of-the-antipodal-two-sphere-mapping-torus.md)

$$
\boxed{H^*(X;\mathbb Z)=\mathbb Z[t,u]/(t^2,tu,u^2,2u),\qquad |t|=1,\ |u|=3.}
$$

Modulo two, $A^*$ is the identity on fiber cohomology. The cohomological [Wang sequence](../../../../../wang-sequence.md) shows that restriction $H^2(X;\mathbb F_2)\to H^2(S^2;\mathbb F_2)$ is onto; choose $y$ mapping to its generator. The classes $1,y$ restrict to a fiber basis, so the [Leray-Hirsch theorem](../../../../../leray-hirsch-theorem.md) makes the total cohomology free over $H^*(S^1;\mathbb F_2)$ on those two classes. Write $\bar t$ for the mod-two base class. The basis is $1,\bar t,y,\bar t y$, and in particular $\bar t y\ne0$. Since $\bar t^2=0$ by pullback and $y^2=0$ by dimension, the [mod-two cohomology ring of the antipodal two-sphere mapping torus](../../../../../mod-two-cohomology-ring-of-the-antipodal-two-sphere-mapping-torus.md) is

$$
\boxed{H^*(X;\mathbb F_2)=\mathbb F_2[\bar t,y]/(\bar t^2,y^2),\qquad |\bar t|=1,\ |y|=2.}
$$

The argument of Question 3 works over any field, so its use here over $\mathbb F_2$ is justified. The ring agrees with that of $S^1\times S^2$; a cohomology ring alone does not determine orientability.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 16](../../paper-16-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
