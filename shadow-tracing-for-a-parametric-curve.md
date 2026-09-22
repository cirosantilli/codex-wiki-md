# Shadow tracing for a parametric curve

↑ **Parent:** [Parametric surface interrogation](parametric-surface-interrogation.md)

From a point light source $P$, a caster point $C(t)$ projects onto a receiving surface along the displayed ray. On a regular transverse branch, differentiating gives $[S_u,S_v,-(C-P)](u',v',\alpha')^T=\alpha C'$. [Newton method](newton-s-method-in-optimization.md) correction and certified patch/curve bounds support continuation and isolation of all visible branches. If the shadow's second [derivative](derivative.md) is bounded by $M$ on an interval of width $h$, its chord error is at most $Mh^2/8$. A fixed sample grid can miss entire shadow components; surface boundaries, occlusion changes and grazing rays require explicit treatment.

## ↑ Ancestors (8)

1. [Parametric surface interrogation](parametric-surface-interrogation.md)
2. [Parametric surface](parametric-surface.md)
3. [Smooth surface](smooth-surface.md)
4. [Differential geometry](differential-geometry-split.md)
5. [Geometry and topology](geometry-and-topology-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/iii/paper-70/5/ii/solution.md)
