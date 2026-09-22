<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

A [subdivision surface](../../../../../subdivision-surface.md) enquiry acts on the limit surface, not just on the current control mesh. The basic [subdivision surface interrogation](../../../../../subdivision-surface-interrogation.md) operations are: enumerate initial patches and their topological adjacency; subdivide a patch into covering children with inherited boundary links; return conservative [bounding volumes](../../../../../bounding-volume.md); estimate approximation error and, where available, normal variation; and evaluate limit positions and first derivatives or tangent data. Boundaries, creases and [extraordinary subdivision vertices](../../../../../extraordinary-subdivision-vertex.md) need explicit rules. Nonnegative convex subdivision weights can supply a local control-hull enclosure, but a scheme with negative weights needs another proved enclosure; an arbitrary control-mesh box is not automatically a bound on the limit.

The [intersection of subdivision limit surfaces](../../../../../intersection-of-subdivision-limit-surfaces.md) can be computed by a paired recursive search. Start with every relevant pair of root patches $(A,B)$, along with their domains and adjacency identifiers:

- If the certified bounding volumes of $A$ and $B$ are disjoint, discard the pair: their limit patches cannot intersect.
- Otherwise refine the larger or less accurately approximated patch, replace the pair by its child pairs and repeat. Subdivide both when their scales are comparable. Preserve cross-patch adjacency information throughout the recursion.
- When the two patches are sufficiently small and flat, form their approximating triangles or planar facets. For transverse configurations with verified error and normal bounds, triangle intersections give candidate line segments and seed locations. Empty polygonal intersection is not by itself an exclusion certificate for the true surfaces: near tangencies, close parallel patches or tiny internal loops require further subdivision or a validated test on the limit functions.
- Correct the candidates onto both limit surfaces using limit-point and tangent enquiries, for example a local parameter chart and the predictor-corrector equations for [transversal intersection of two parametric surfaces](../../../../../transversal-intersection-of-two-parametric-surfaces.md). Continue each resolved arc through adjacent leaves. Where a chart is unavailable, keep refining and produce an enclosure with a proved error bound rather than claim an exact point from the mesh.
- Join arc endpoints using patch/parameter adjacency and verified shared-boundary matches, remove duplicate segments from adjacent patch pairs, orient each component and assemble the resulting open curves and closed loops. Purely spatial proximity is not enough to join two distinct nearby branches.

A termination criterion specifies geometric error and conditioning, not merely a fixed refinement depth. For isolated regular transverse components, shrinking limit enclosures and normal/error bounds permit reliable curve approximation. Candidate boxes cannot be discarded merely because no coarse edge has crossed another surface: a complete small closed component can lie in the interior. Tangency, coincident limit patches, creases and poorly conditioned extraordinary-point neighborhoods need special tests or must be reported as unresolved degenerate configurations. **The intersection is that of the two subdivision limits; intersecting a finite refined mesh without error control only gives an approximation.**

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 56](../../paper-56-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
