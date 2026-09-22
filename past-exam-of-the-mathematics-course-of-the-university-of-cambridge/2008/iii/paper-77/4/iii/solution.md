<h1 id="4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Treat the [subdivision surface](../../../../../../subdivision-surface.md) as an evaluable limit together with its refinement hierarchy. At a requested location $\xi$, evaluate the limit position $S(\xi)$ and two independent limit [tangent vectors](../../../../../../tangent-vector.md), then set

$$
\boxed{S_d(\xi)=S(\xi)+d\,\frac{S_1(\xi)\times S_2(\xi)}{\lVert S_1(\xi)\times S_2(\xi)\rVert}.}
$$

On regular regions, local spline patches supply position and derivative evaluations. Near extraordinary vertices, use the actual subdivision rule and its limit-position and tangent evaluation machinery, or a convergent local refinement with controlled position and [normal vector](../../../../../../normal-vector.md) errors. If a tangent pair degenerates, the regular offset evaluator is not defined there; a crease requires separate one-sided offsets and an explicitly chosen join.

For polygonal interrogation, subdivide the base mesh adaptively. At every new sample, evaluate the base limit and its limit [normal vector](../../../../../../normal-vector.md), and displace that sample by $d n$. Connect these samples with the inherited connectivity, refining until flatness and normal-variation bounds meet the desired tolerance. If the position error is $\delta$ and unit-normal error is $\eta$, the offset-position error is at most $\delta+|d|\eta$, in addition to the interpolation error between samples. A [variable normal offset](../../../../../../variable-normal-offset.md) can be sampled at the same locations, with its approximation error included as well. The result retains the base subdivision hierarchy for locating points and refining patches.

Displacing the original control vertices along estimated vertex normals and applying the original [subdivision mask](../../../../../../subdivision-mask.md) just once does not, in general, give the exact [surface offset](../../../../../../parallel-surface.md). If $A$ is one linear refinement step, then $A(P+d n(P))=AP+d A n(P)$, while displacing the refined base gives $AP+d n(AP)$; normalization and the normal calculation are nonlinear, so $A n(P)\ne n(AP)$ in general. Thus the exact offset is an interrogation wrapper around the base limit, and a conventional subdivision control mesh for it is a fitted approximation requiring refinement or error control. **Refine and interrogate the base limit, then offset its evaluated points; do not assume offsetting commutes with subdivision.**

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [Paper 77](../../../paper-77-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
