<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

First take $k\ge2$, so the simple-knot [B-splines](../../../../../b-spline.md) are continuous, vanish at both [support](../../../../../support.md) endpoints, and are strictly positive inside their [supports](../../../../../support.md). Thus the diagonal condition is $t_i<x_i<t_{i+k}$. We prove both directions of the [Schoenberg–Whitney theorem](../../../../../schoenberg-whitney-theorem.md), deriving the weighted zero-count fact needed for sufficiency rather than relying on an ambiguous [coefficient](../../../../../coefficient.md)-free hint.

For necessity, suppose $N_i(x_i)=0$. If $x_i\le t_i$, then for every row $r\le i$ and column $j\ge i$ we have $x_r\le x_i\le t_i\le t_j$, hence $N_j(x_r)=0$. The first $i$ rows have nonzero entries in at most $i-1$ columns and are linearly dependent. If instead $x_i\ge t_{i+k}$, then for $r\ge i$ and $j\le i$ we have $x_r\ge x_i\ge t_{i+k}\ge t_{j+k}$, so those entries vanish. The last $n-i+1$ rows have nonzero entries in at most $n-i$ columns and are again dependent. In either case the [B-spline collocation matrix](../../../../../b-spline-collocation-matrix.md) is singular. Thus invertibility implies the diagonal positivity condition.

We establish two elementary [spline](../../../../../spline-mathematics.md) facts for the converse. For [local linear independence of B-splines](../../../../../local-linear-independence-of-b-splines.md), extend the strictly increasing knots in both directions. On a cell $(t_j,t_{j+1})$ the $k$ active [basis](../../../../../basis.md) functions have indices $j-k+1,\ldots,j$. Their knot [polynomials](../../../../../polynomial-split.md) are $\psi_i(y)=\prod_{\ell=1}^{k-1}(y-t_{i+\ell})$. The [Cox-de Boor recurrence](../../../../../cox-de-boor-recursion-formula.md) proves [Marsden's identity](../../../../../marsden-identity.md)

$$
(y-x)^{k-1}=\sum_{i=j-k+1}^jN_i(x)\psi_i(y).
$$

Here is the induction behind that identity. For order one the indicator functions sum to one. On passing from order $k-1$ to $k$, collect the [coefficient](../../../../../coefficient.md) of each lower-order [basis](../../../../../basis.md) function. With $u=t_i$, $v=t_{i+k-1}$, its extra factor is

$$
\frac{(x-u)(y-v)+(v-x)(y-u)}{v-u}=y-x.
$$

Thus the identity at one order multiplies by $y-x$ at the next.

The $k$ [polynomials](../../../../../polynomial-split.md) $\psi_i$ are independent: evaluate successively at $y=t_j,t_{j-1},\ldots,t_{j-k+1}$. The first evaluation isolates $\psi_j$; after its [coefficient](../../../../../coefficient.md) has been eliminated the next isolates $\psi_{j-1}$, and so on, with nonzero diagonal factors because the knots are distinct. Comparing powers of $y$ in the identity then shows that the active $N_i$ span all [polynomials](../../../../../polynomial-split.md) of degree at most $k-1$ on the cell. There are $k$ of them, so they are independent. In particular, a [spline](../../../../../spline-mathematics.md) vanishes on a whole open cell exactly when all its active [coefficients](../../../../../coefficient.md) vanish. Padding the finite [coefficient](../../../../../coefficient.md) vector with zeros makes this fact apply also near the outer knots.

Next let $s=\sum_{i=p}^qc_iN_i$ be a real [spline](../../../../../spline-mathematics.md) on $I=(t_p,t_{q+k})$, with no identically zero knot cell there. The [simple-knot B-spline regularity](../../../../../simple-knot-b-spline-regularity.md) gives $s\in C^{k-2}$, and its [derivatives](../../../../../derivative.md) through order $k-2$ vanish at both endpoints because it is supported on the closed interval. Suppose it has $Z$ distinct interior zeros. Its zero set initially has $Z+2$ [connected components](../../../../../connected-component.md), counting the endpoints; the zeros are isolated because no cell vanishes identically.

A useful form of [Rolle's theorem](../../../../../rolle-theorem.md) counts zero components, including any zero intervals that arise after differentiation. Between two successive zero components a real differentiable function is nonzero and has an interior extremum, supplying a zero of its [derivative](../../../../../derivative.md). These [derivative](../../../../../derivative.md)-zero components are distinct: a zero interval connecting two such extrema would make the original function constant across an intervening zero and nonzero gap, which is impossible. If its [derivative](../../../../../derivative.md) also vanishes at both endpoints, those supply two further distinct components. Thus differentiation increases the zero-component count by at least one. Apply this successively through [derivative](../../../../../derivative.md) order $k-2$; every required endpoint [derivative](../../../../../derivative.md) vanishes. No [derivative](../../../../../derivative.md) in this process can vanish identically: that would make $s$ a global [polynomial](../../../../../polynomial-split.md) of degree below $k-1$, with all its endpoint [derivatives](../../../../../derivative.md) through that degree zero, forcing $s=0$. The final [derivative](../../../../../derivative.md) has at least $Z+k$ zero components.

That final [derivative](../../../../../derivative.md) is continuous and piecewise affine on $q-p+k$ knot cells. Each closed affine cell can meet at most one zero component: two different zeros would force the whole cell to vanish, joining them into one component. Every zero component meets a cell, so there are at most $q-p+k$ of them. For $k=2$ this argument applies directly without differentiation. We have proved the [compact-support spline zero count](../../../../../compact-support-spline-zero-count.md)

$$
\boxed{Z(s;I)\le q-p.}
$$

This proof also accommodates zero intervals of the [derivatives](../../../../../derivative.md); counting them as infinitely many distinct zeros would invalidate a naive repeated-Rolle argument.

Now assume $N_i(x_i)>0$ for all $i$ and suppose $A_xc=0$ for a nonzero [coefficient](../../../../../coefficient.md) vector. Since $A_x$ is real, a nonzero real null vector can be chosen. Set $s=\sum_ic_iN_i$, so $s(x_i)=0$ for all $i$. Consider one [connected component](../../../../../connected-component.md) of the union of the open [supports](../../../../../support.md) of the terms with $c_i\ne0$. If its first and last indices are $p,q$, the component is exactly $I=(t_p,t_{q+k})$. On this interval $s$ equals $s_0=\sum_{i=p}^qc_iN_i$. Each knot cell in $I$ has at least one active nonzero [coefficient](../../../../../coefficient.md), so local independence ensures $s_0$ does not vanish on any whole cell.

For every $p\le i\le q$, diagonal positivity gives $t_i<x_i<t_{i+k}$, and this places $x_i$ inside $I$. Thus $s_0$ has the $q-p+1$ distinct zeros $x_p,\ldots,x_q$, contradicting the upper bound $q-p$. There is no nonzero null vector, proving sufficiency. Together the two directions give

$$
\boxed{A_x\text{ is invertible}\quad\Longleftrightarrow\quad N_i(x_i)>0\text{ for every }i.}
$$

For completeness, order $k=1$ consists of disjoint interval indicators, with the usual left-closed, right-open convention. An invertible ordered collocation requires exactly one site in each interval; ordering makes this equivalent to $N_i(x_i)>0$, and the [matrix](../../../../../matrix.md) is then the identity. This handles possible sites at left knots without incorrectly replacing positivity by a strict interior inequality for order one.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 71](../../paper-71-split.md)
3. [Iii](../../split.md)
4. [2004](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
