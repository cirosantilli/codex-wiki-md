<h1 id="24h/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

**The literal assertion needs $q\ne p$.** If $q=p$, the two [geodesic circles](../../../../../../geodesic-circle.md) coincide, have equal tangent lines at every point, and do not intersect transversally; their intersection is not finite. We prove that [close geodesic circles intersect twice](../../../../../../close-geodesic-circles-intersect-twice.md) for nearby distinct centres, and in fact find exactly two intersections.

Choose a strongly convex normal neighbourhood about $p$ and a sufficiently small $r>0$ so that every circle considered and all [geodesics](../../../../../../geodesic.md) joining its points to nearby centres remain there. Squared distance $d(q,x)^2$ is then smooth in both arguments, and the [exponential map](../../../../../../exponential-map-riemannian-geometry.md) is nonsingular on the relevant radius-$r$ tangent circles. Consequently all these distance spheres are smooth embedded one-dimensional manifolds.

Write $q=\exp_p(\varepsilon v)$ with $|v|=1$ and $\varepsilon>0$, and parameterize $S_r(p)$ by $x(\theta)=\exp_p(re(\theta))$. Define

$$
F(\varepsilon,v,\theta)=d(\exp_p(\varepsilon v),x(\theta))^2-r^2.
$$

The first variation of [geodesic](../../../../../../geodesic.md) energy gives

$$
\partial_\varepsilon F(0,v,\theta)=-2r\langle v,e(\theta)\rangle.
$$

Indeed differentiating the energy of the joining [geodesic](../../../../../../geodesic.md) cancels the interior term by the [geodesic](../../../../../../geodesic.md) equation, leaving the initial endpoint term $-2\langle re(\theta),v\rangle$. This is also the endpoint form of the [Gauss lemma](../../../../../../gauss-s-lemma-riemannian-geometry.md).

Since $F(0,v,\theta)=0$, the quotient $F/\varepsilon$ extends smoothly to $\varepsilon=0$ by integrating $\partial_\varepsilon F$ from zero to $\varepsilon$. At zero it is $-2r\cos(\theta-\arg v)$, with exactly two simple zeros. The [implicit function theorem](../../../../../../implicit-function-theorem.md) gives two nearby simple zeros for small positive $\varepsilon$. [Compactness](../../../../../../compact-space.md) of the unit vector circle makes the choice of small $\varepsilon$ uniform in $v$; away from fixed neighbourhoods of those two zeros the cosine is bounded away from zero, so there are no additional zeros.

A nonzero angular derivative at either zero says that the defining function of $S_r(q)$ has a nonzero derivative along $S_r(p)$. Thus their tangent lines differ: the intersections are transverse. Shrinking the neighbourhood of centres accordingly proves

$$
\boxed{\#(S_r(p)\cap S_r(q))=2,\qquad
\#(S_r(p)\cap S_r(q))\equiv0\pmod2
\quad(q\ne p,\ q\text{ sufficiently near }p).}
$$

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [24H](../../24h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
