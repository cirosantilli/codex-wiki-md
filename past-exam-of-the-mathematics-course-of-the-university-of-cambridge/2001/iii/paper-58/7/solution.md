<h1 id="7/solution">Solution</h1>

↑ **Parent:** [7](../7.md)

Fix a clamped nondecreasing [spline knot sequence](../../../../../spline-knot-sequence.md) $t_1,\ldots,t_{n+k}$ on $[a,b]$, with $t_1=\cdots=t_k=a$ and $t_{n+1}=\cdots=t_{n+k}=b$. For continuous [splines](../../../../../spline-mathematics.md) assume interior multiplicities at most $k-1$, and assume $t_i<t_{i+k}$. An order-$k$ [spline](../../../../../spline-mathematics.md) has degree at most $k-1$ on each nonempty knot interval; at a knot of multiplicity $r$ it has $k-1-r$ continuous [derivatives](../../../../../derivative.md). Its dimension is $n$, and a normalized [B-spline](../../../../../b-spline.md) [basis](../../../../../basis.md) $N_1,\ldots,N_n$ has local [support](../../../../../support.md), nonnegative values and sum one on $[a,b]$.

These properties are visible in the [Cox-de Boor recurrence](../../../../../cox-de-boor-recursion-formula.md). Starting with interval indicators at order one, set

$$
N_{i,k}(x)=\frac{x-t_i}{t_{i+k-1}-t_i}N_{i,k-1}(x)+\frac{t_{i+k}-x}{t_{i+k}-t_{i+1}}N_{i+1,k-1}(x),
$$

with a term of zero denominator defined to be zero. On each contributing [support](../../../../../support.md) the weights are nonnegative, and summing the recurrence makes the coefficients of each lower-order [B-spline](../../../../../b-spline.md) add to one. This gives partition of unity and $\operatorname{supp}N_{i,k}=[t_i,t_{i+k}]$, with endpoint values defined by limits.

At distinct ordered sites $x_1<\cdots<x_n$, interpolation is the [linear system](../../../../../system-of-linear-equations.md)

$$
A_{\mathbf x}c=y,\qquad (A_{\mathbf x})_{ij}=N_j(x_i).
$$

It has a unique solution for every data [vector](../../../../../vector.md) exactly when the [B-spline collocation matrix](../../../../../b-spline-collocation-matrix.md) is invertible. The [Schoenberg–Whitney theorem](../../../../../schoenberg-whitney-theorem.md) characterizes this by $N_i(x_i)>0$ for every $i$; away from clamped endpoints this is $t_i<x_i<t_{i+k}$. At the clamped endpoints the first and last [B-splines](../../../../../b-spline.md) have value one, so the endpoint version uses this positive-value formulation rather than the strict inequalities. Both ordering and the support conditions matter. A [spline](../../../../../spline-mathematics.md) space with interior knots is generally not a [Chebyshev system](../../../../../chebyshev-system.md) on the entire interval: a locally supported [B-spline](../../../../../b-spline.md) vanishes on an interval. Thus arbitrary distinct nodes need not permit interpolation. Merely specifying all data sites as knots also need not fix the remaining freedom; for example, cubic interpolation with simple interior knots at $m-2$ data sites has dimension $m+2$, and two extra boundary conditions are needed to interpolate $m$ values uniquely.

The positivity governing this existence theorem is [total nonnegativity of B-spline collocation matrices](../../../../../total-nonnegativity-of-b-spline-collocation-matrices.md): every square minor with increasing row and column indices is nonnegative. In spline terminology this is often called total positivity, but it permits zero minors caused by disjoint [supports](../../../../../support.md). It is not the stronger assertion that every minor is strictly positive. A useful proof uses [knot insertion](../../../../../knot-insertion.md). Each refinement step changes [coefficients](../../../../../coefficient.md) by

$$
\widetilde c_j=\alpha_jc_j+(1-\alpha_j)c_{j-1},\qquad 0\le\alpha_j\le1,
$$

with the unchanged endpoint pieces. The refinement [matrix](../../../../../matrix.md) is nonnegative bidiagonal, and its minors are nonnegative: any nonzero determinant has its allowed diagonal matching and is a product of nonnegative entries. Products preserve this property by the [Cauchy–Binet formula](../../../../../cauchy-binet-formula.md). Insert each sampling site to full multiplicity, so evaluation at that site becomes selection of an ordered refined [coefficient](../../../../../coefficient.md). The collocation [matrix](../../../../../matrix.md) is then an ordered row submatrix of the refinement product, proving total nonnegativity. The strict support criterion is the strict part of this argument: an ordered path through the consecutive support intervals exists exactly when every diagonal [B-spline](../../../../../b-spline.md) value is positive, giving the [Schoenberg–Whitney theorem](../../../../../schoenberg-whitney-theorem.md) determinant criterion.

If $A$ is invertible, its determinant is positive and the [adjugate identity](../../../../../adjugate-identity.md) yields

$$
(A^{-1})_{ij}=(-1)^{i+j}\frac{\det A_{\widehat j,\widehat i}}{\det A},\qquad(-1)^{i+j}(A^{-1})_{ij}\ge0.
$$

This [checkerboard inverse of a totally nonnegative matrix](../../../../../checkerboard-inverse-of-a-totally-nonnegative-matrix.md) is the central stability fact. With alternating data $e_i=(-1)^i$, the absolute row sums satisfy

$$
|(A^{-1}e)_j|=\sum_i|(A^{-1})_{ji}|,\qquad\|A^{-1}\|_\infty=\|A^{-1}e\|_\infty.
$$

For general data, the cardinal [splines](../../../../../spline-mathematics.md) are $\ell_i(x)=\sum_jN_j(x)(A^{-1})_{ji}$. The [spline interpolation operator](../../../../../spline-interpolation-operator.md) and its exact [Lebesgue constant of interpolation](../../../../../lebesgue-constant-of-interpolation.md) are

$$
P_{\mathbf x}f=\sum_if(x_i)\ell_i,\qquad\|P_{\mathbf x}\|=\Lambda_{\mathbf x}:=\max_x\sum_i|\ell_i(x)|\le\|A_{\mathbf x}^{-1}\|_\infty.
$$

The equality for the [operator norm](../../../../../operator-norm.md) follows by extending the signs at distinct sites to a continuous unit-norm data [function](../../../../../function-split.md), as in Solution 2. That solution also shows the last inequality can be very strict. Stability concerns the range [function](../../../../../function-split.md) as well as its [coefficients](../../../../../coefficient.md).

An optimal interpolation set must be specified relative to an objective. For the normalized [B-spline](../../../../../b-spline.md) [coefficients](../../../../../coefficient.md), every admissible sampling set satisfies

$$
\kappa(\mathcal S)\le\|A_{\mathbf x}^{-1}\|_\infty,
$$

since $c(s)=A_{\mathbf x}^{-1}(s(x_i))$ and sampling cannot increase the [supremum norm](../../../../../supremum-norm.md). If a unit-norm [spline](../../../../../spline-mathematics.md) $s_*$ has $n$ ordered alternating extrema $s_*(x_i)=(-1)^i$ at admissible sites, the checkerboard identity gives

$$
|c_j(s_*)|=\sum_i|(A_{\mathbf x}^{-1})_{ji}|.
$$

Taking the largest row shows $\|A_{\mathbf x}^{-1}\|_\infty\le\kappa(\mathcal S)$, so equality holds. This proves the [optimal spline coefficient interpolation sites](../../../../../optimal-spline-coefficient-interpolation-sites.md) property and the [Chebyshev spline coefficient and dual norm equality](../../../../../chebyshev-spline-coefficient-and-dual-norm-equality.md). In particular, for the cubic space of Solution 1 the alternating extrema $-1,-2/3,0,2/3,1$ satisfy the support conditions. Its [coefficients](../../../../../coefficient.md) have maximum magnitude $11/2$, so these sites are optimal for coefficient recovery and

$$
\boxed{\kappa(\mathcal S)=\frac{11}{2}=\|A_{\mathbf x}^{-1}\|_\infty\quad\text{at those five sites}.}
$$

The argument proves optimality whenever this admissible equioscillating [spline](../../../../../spline-mathematics.md) is available; it does not identify extrema of an arbitrary [spline](../../../../../spline-mathematics.md) as optimal sites, or transfer coefficient optimality automatically to the [Lebesgue constant of interpolation](../../../../../lebesgue-constant-of-interpolation.md).

For the intrinsic interpolation objective, minimize $\Lambda_{\mathbf x}$ itself. There is a minimizer for a fixed finite-dimensional continuous [spline](../../../../../spline-mathematics.md) space. Indeed the sites lie in a compact ordered simplex. On admissible sets, inverse entries and hence $\Lambda_{\mathbf x}$ vary continuously. As a collocation [matrix](../../../../../matrix.md) tends to a singular one, its inverse [norm](../../../../../norm.md) diverges. The [uniform-norm stability of a B-spline basis](../../../../../uniform-norm-stability-of-a-b-spline-basis.md) gives the complementary bound

$$
\|P_{\mathbf x}\|\ge\frac{\|A_{\mathbf x}^{-1}\|_\infty}{\kappa(\mathcal S)}:
$$

choose sample signs attaining a largest inverse row, extend them to a continuous unit-norm [function](../../../../../function-split.md), and use $\|Tc\|_\infty\ge\|c\|_\infty/\kappa(\mathcal S)$. Thus a minimizing sequence with bounded [Lebesgue constants of interpolation](../../../../../lebesgue-constant-of-interpolation.md) cannot approach a singular site set. A convergent subsequence has an admissible limit attaining the minimum.

[Fekete interpolation sites for a continuous function space](../../../../../fekete-interpolation-sites-for-a-continuous-function-space.md) offer another useful, constructive criterion: maximize the absolute evaluation determinant. A nonzero maximum exists by compactness and linear independence. Replacing one row by evaluation at $x$ multiplies the determinant by the corresponding cardinal [function](../../../../../function-split.md), so maximality gives $|\ell_i(x)|\le1$, and therefore $\Lambda_{\mathbf x}\le n$. These sites are determinant-optimal, with a proven interpolation bound; one should not claim without further argument that they minimize $\Lambda_{\mathbf x}$. [Greville abscissae](../../../../../greville-abscissa.md) provide inexpensive admissible sites for the usual continuous clamped [spline](../../../../../spline-mathematics.md) spaces of order at least two. Admissibility alone does not give the best stability bound.

Finally, the [coefficient condition number of a normalized B-spline basis](../../../../../coefficient-condition-number-of-a-normalized-b-spline-basis.md) is bounded by a constant depending only on order. To see the mechanism, for each [coefficient](../../../../../coefficient.md) choose a longest nonempty knot cell in that [B-spline](../../../../../b-spline.md)'s support. If its length is $h$ and the support width is $W$, then $W/h\le k$. On that cell the [spline](../../../../../spline-mathematics.md) is a degree-at-most-$k-1$ [polynomial](../../../../../polynomial-split.md); repeated [Markov polynomial inequalities](../../../../../markov-inequality-for-polynomial-derivatives.md) bound its $r$th [derivative](../../../../../derivative.md) by $C_kh^{-r}\|s\|_\infty$. In the [De Boor–Fix spline coefficient functional](../../../../../de-boor-fix-spline-coefficient-functional.md), the accompanying derivative of the knot [polynomial](../../../../../polynomial-split.md) is bounded by $C_kW^r$. Each term is consequently at most $C_k(W/h)^r\|s\|_\infty$, yielding $\|c(s)\|_\infty\le C_k\|s\|_\infty$ independently of the number and spacing of knots. This is basis stability; it does not bound $\|A_{\mathbf x}^{-1}\|$ at arbitrarily poor sampling sites.

For approximation, reproduction gives the [Lebesgue inequality for approximation projectors](../../../../../polynomial-reproduction-error-bound.md)

$$
\|f-P_{\mathbf x}f\|_\infty\le(1+\Lambda_{\mathbf x})\inf_{s\in\mathcal S}\|f-s\|_\infty.
$$

As the maximum knot gap tends to zero with fixed order, [spline quasi-interpolation](../../../../../spline-quasi-interpolation.md) gives an approximant with error at most $\omega(f,kh)$, so the infimum tends to zero. A sequence of uniformly bounded interpolation [linear operators](../../../../../linear-operator.md) therefore converges to every continuous target. Local [support](../../../../../support.md) and a stable choice of sites make [spline interpolation](../../../../../spline-interpolation.md) effective; mesh refinement without control of the interpolation [operator norm](../../../../../operator-norm.md) is not by itself a convergence proof.

## ↑ Ancestors (10)

1. [7](../7.md)
2. [Paper 58](../../paper-58-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
