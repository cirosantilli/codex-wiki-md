# Recursive half-space clipping of a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](subdivision-curve-interrogation.md)

For an oriented plane function $\ell$, certified extrema over a [bounding volume](bounding-volume.md) allow a [subdivision curve](subdivision-curve.md) piece to be rejected when $\max\ell<0$, or wholly retained when $\min\ell\geq0$. Otherwise subdivide. At an explicitly chosen rendering tolerance, a sufficiently flat, sufficiently short piece can be replaced by its clipped chord. This is an approximation, not a proof of exact crossing topology. Exact treatment of tangent contacts and small excursions requires root isolation of $\ell(C(t))$ and splitting into sign-constant intervals, when the curve representation supports such isolation.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2006/iii/paper-66/4/b/solution.md)
