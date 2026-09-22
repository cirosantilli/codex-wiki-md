# Closest-point search on a subdivision curve

↑ **Parent:** [Subdivision curve interrogation](subdivision-curve-interrogation.md)

At a regular differentiable interior nearest point of a [parametric curve](parametric-curve.md), the displacement from the query point is perpendicular to the [tangent vector](tangent-vector.md). A [branch and bound](branch-and-bound.md) search uses distances to certified enclosing [bounding volumes](bounding-volume.md) as lower bounds, and evaluated limit points as upper bounds. Refine the most promising restricted pieces until the upper bound differs from the global lower bound by the chosen distance tolerance. Safeguarded [Newton root-finding iteration](newton-root-finding-iteration.md) accelerates local candidates, but endpoints, nonregular points, ties and other stationary branches must not be omitted.

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

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-59/2/solution.md)
