<h1 id="de-boor-fix-spline-coefficient-functional">De Boor–Fix spline coefficient functional</h1>

↑ **Parent:** [Marsden dual functional](marsden-dual-functional.md)

This [linear functional](linear-functional.md) extracts one [coefficient](coefficient.md) of a [B-spline](b-spline.md) expansion using local [polynomial](polynomial-split.md) data. With $\psi_i(x)=\prod_{\ell=1}^{k-1}(x-t_{i+\ell})/(k-1)!$ and a point $\xi$ inside a knot cell in the [support](support.md), it is $\sum_{r=0}^{k-1}(-1)^rs^{(r)}(\xi)\psi_i^{(k-1-r)}(\xi)$. The local [polynomial](polynomial-split.md) identity for the [Marsden dual functional](marsden-dual-functional.md) gives the desired [coefficient](coefficient.md). Its bounded restriction to the local [spline](spline-mathematics.md) space can be extended to continuous data on $[t_i,t_{i+k}]$ by the [Hahn-Banach theorem](hahn-banach-theorem.md), with the same bound. Such extensions supply [spline quasi-interpolation](spline-quasi-interpolation.md) [coefficients](coefficient.md) without requiring [derivatives](derivative.md) of the data.

## ↑ Ancestors (10)

1. [Marsden dual functional](marsden-dual-functional.md)
2. [Marsden identity](marsden-identity.md)
3. [B-spline](b-spline.md)
4. [Spline approximation](spline-approximation.md)
5. [Spline (mathematics)](spline-mathematics.md)
6. [Uniform approximation](uniform-approximation-split.md)
7. [Analysis](analysis-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/1/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-58/7/solution.md)
