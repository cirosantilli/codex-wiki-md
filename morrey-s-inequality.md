<h1 id="morrey-s-inequality">Morrey's inequality</h1>

↑ **Parent:** [Sobolev embedding theorem](sobolev-embedding-theorem.md)

For $d<p<\infty$, every [Sobolev space](sobolev-space-split.md) element $u\in W^{1,p}(\mathbb R^d)$ has a [Hölder continuous function](holder-condition.md) representative of exponent $1-d/p$, with the displayed bound. It also satisfies $\|u\|_\infty\leq C_{d,p}(\|u\|_p+\|\nabla u\|_p)$. Averaging the [fundamental theorem of calculus along a line segment](fundamental-theorem-of-calculus-along-a-line-segment.md) over a ball gives

$$
|u(x)-u_{B(x,r)}|\leq C_d\int_{B(x,r)}\frac{|\nabla u(z)|}{|x-z|^{d-1}}\,dz.
$$

The [Holder inequality](holder-inequality.md) bounds this by $C_{d,p}r^{1-d/p}\|\nabla u\|_p$, because $(d-1)p'<d$. To compare two ball averages, translate a ball along the segment between their centres and use the same [fundamental theorem of calculus along a line segment](fundamental-theorem-of-calculus-along-a-line-segment.md). These bounds give the displayed estimate. [Density of smooth functions in a Sobolev space](density-of-smooth-functions-in-a-sobolev-space.md) supplies the representative for nonsmooth $u$. For $p=\infty$, the corresponding conclusion is [Lipschitz continuity](lipschitz-continuity.md).

## ↑ Ancestors (7)

1. [Sobolev embedding theorem](sobolev-embedding-theorem.md)
2. [Sobolev space](sobolev-space-split.md)
3. [Functional analysis](functional-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (7)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-68/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105/2/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105/2/b/ii/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-105/2/c/solution.md)
- [Screened sine-Gordon energy](screened-sine-gordon-energy.md)
- [Sobolev slicing and planar continuity](sobolev-slicing-and-planar-continuity.md)
