<h1 id="5/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Without the separation assumptions, explicitly test whether the caster lies between the light and receiver: roots with $0<\alpha\leq1$ are not receiver points shadowed by that caster point, and $\alpha<0$ belongs to the backward ray. The light can lie on the curve, making $C(t)-P=0$, or a ray can run along rather than cut the surface; both need exceptional treatment.

Without the facing assumption, allow back-facing regions, tangencies with singular continuation Jacobian, folds, multiple ray intersections, self-occlusion and changes of the visible first intersection. Visibility can create or delete whole shadow branches or switch them between receiver sheets. Also handle open boundaries, trimmed holes, disconnected receivers, closed casting loops, caster/receiver intersections and a light inside a closed receiver. Subdivision and intersection isolation must precede branch continuation near these events; normals, orientation and sorted ray distances decide which solutions are physically visible. The output can be several point sequences, rather than one connected polyline.

## ↑ Ancestors (11)

1. [Iii](../iii.md)
2. [5](../../5.md)
3. [Paper 70](../../../paper-70-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
