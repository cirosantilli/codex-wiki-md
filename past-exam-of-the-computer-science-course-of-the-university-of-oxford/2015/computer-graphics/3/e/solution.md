<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

At each primary hit $p$, send a [shadow ray](../../../../../shadow-ray.md) toward each point light. An especially clear parameterization is

$$
s_j(t)=p+t(\ell_j-p),\qquad 0<t<1.
$$

If an opaque scene surface intersects this open segment, the source is hidden. The finite interval is essential: an object beyond the light must not cast a shadow at $p$. Exclude the launch surface with a small geometrically appropriate origin offset or positive minimum parameter, so [floating-point arithmetic](../../../../../floating-point-arithmetic-split.md) does not create a false self-intersection.

Introduce a visibility factor $V_j(p)$ equal to zero when blocked and one otherwise. The modified equation is

$$
\boxed{I(p)=k_aI_a+\sum_j V_j(p)I_j(p)\left[k_d\max(0,\hat N\cdot\hat L_j)+k_s\chi_j\max(0,\hat R_j\cdot\hat V)^n\right].}
$$

A blocked light loses both its diffuse and specular contributions. The simple ambient approximation remains. Opaque point lights produce hard shadow boundaries. Use a consistent sidedness policy for occluders: an opaque closed solid blocks from either crossing side, so a two-sided blocker test is appropriate even when primary visibility uses [back-face culling](../../../../../back-face-culling.md). An any-hit query can stop as soon as it finds one blocker before the light.

## ↑ Ancestors (11)

1. [E](../e.md)
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
