# Shadow tracing for a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](subdivision-curve-interrogation.md)

For a point light at $L$, the shadow of a curve point is the first surface intersection on its ray beyond that point. Certified patch bounds and subdivision isolate intersections; regular hits are corrected with a three-variable [Newton method](newton-s-method-in-optimization.md) solve. Differentiating the displayed equation gives $[S_u,S_v,-(C-L)](u',v',\lambda')^T=\lambda C'$, a predictor for continuation along the shadow. Surface boundaries and grazing rays require clipping and reseeding; every visible component must be isolated, rather than assumed detectable from a fixed sample of the casting curve.

## ↑ Ancestors (8)

1. [Subdivision curve interrogation](subdivision-curve-interrogation.md)
2. [Subdivision curve](subdivision-curve.md)
3. [Computer aided geometric design](computer-aided-geometric-design.md)
4. [Numerical analysis](numerical-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-66/6/iii/solution.md)
