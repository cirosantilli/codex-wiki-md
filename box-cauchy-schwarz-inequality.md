# Box Cauchy-Schwarz inequality

↑ **Parent:** [Box norm](box-norm.md)

For four [real-valued functions](real-valued-function.md) on a finite [Cartesian product](cartesian-product.md), let $\Lambda(f_{00},f_{01},f_{10},f_{11})=\mathbb E_{x_0,x_1,y_0,y_1}\prod_{i,j=0}^1 f_{ij}(x_i,y_j)$. Repeated [Cauchy-Schwarz inequalities](cauchy-schwarz-inequality.md) give

$$
|\Lambda(f_{00},f_{01},f_{10},f_{11})|\leq\prod_{i,j=0}^1\|f_{ij}\|_{\square}.
$$

First separate the two $y$ averages and apply [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md) in $(x_0,x_1)$. Each resulting squared factor is $\mathbb E_{y,y'}(\mathbb E_x f(x,y)f(x,y'))(\mathbb E_x g(x,y)g(x,y'))$, bounded by $\|f\|_{\square}^2\|g\|_{\square}^2$ by another [Cauchy-Schwarz inequality](cauchy-schwarz-inequality.md). Expanding the four factors of $f+g$ and applying this inequality to each of the sixteen terms gives the [triangle inequality](triangle-inequality.md) for the [box norm](box-norm.md).

## ↑ Ancestors (6)

1. [Box norm](box-norm.md)
2. [Additive combinatorics](additive-combinatorics-split.md)
3. [Combinatorics](combinatorics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Box norm](box-norm.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-16/3/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-129/4/solution.md)
