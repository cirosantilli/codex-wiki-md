<h1 id="simpson-s-rule">Simpson's rule</h1>

↑ **Parent:** [Quadrature rule](quadrature-rule.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Simpson's_rule)

[Simpson's rule](simpson-s-rule.md) integrates the quadratic interpolant through two endpoints and their midpoint. It is exact also on cubic [polynomials](polynomial-split.md). On $[0,2]$, define the raw kernel $K(t)=L[(x-t)_+^3]$, where $L$ is integral minus the rule. Then $K(t)=-t^3(4-3t)/12$ for $0\leq t\leq1$ and $K(t)=-(2-t)^3(3t-2)/12$ for $1\leq t\leq2$. It is strictly negative inside the interval and integrates to $-1/15$. The [Peano kernel theorem](peano-kernel-theorem.md) therefore gives the sharp bound $|L(f)|\leq\|f^{(4)}\|_\infty/90$; $f(x)=x^4/24$ attains equality. Scaling to endpoint spacing $h$ gives $h^5/90$. The normalized [Peano kernel](peano-kernel.md) is $K/3!$, so the external factorial must be omitted when using that normalization.

## ↑ Ancestors (7)

1. [Quadrature rule](quadrature-rule.md)
2. [Numerical integration](numerical-integration.md)
3. [Numerical analysis](numerical-analysis-split.md)
4. [Analysis](analysis-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/ib/paper-3/19c/solution.md)
- [Simpson's rule](simpson-s-rule.md)
