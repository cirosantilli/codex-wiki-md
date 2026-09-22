<h1 id="de-boor-s-algorithm">De Boor's algorithm</h1>

↑ **Parent:** [B-spline](b-spline.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/De_Boor's_algorithm)

For degree $p$, knots $t_i$ and span $[t_k,t_{k+1})$, initialize $d_j^{(0)}=P_{k-p+j}$ for $0\le j\le p$. At level $r$, update $j=p,p-1,\ldots,r$ by $d_j^{(r)}=(1-\alpha_{j,r})d_{j-1}^{(r-1)}+\alpha_{j,r}d_j^{(r-1)}$, where $\alpha_{j,r}=(t-t_{k-p+j})/(t_{k+1+j-r}-t_{k-p+j})$. The point is $d_p^{(p)}$. This evaluates a [B-spline](b-spline.md) by local affine combinations.

// Target: analysis.bigb

## ↑ Ancestors (8)

1. [B-spline](b-spline.md)
2. [Spline approximation](spline-approximation.md)
3. [Spline (mathematics)](spline-mathematics.md)
4. [Uniform approximation](uniform-approximation-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-77/3/ii/solution.md)
