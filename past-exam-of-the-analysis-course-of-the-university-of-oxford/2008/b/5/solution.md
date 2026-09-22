<h1 id="b/5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the convention that the [inner product](../../../../inner-product-split.md) is linear in its first argument. If $v\ne0$, nonnegativity of $\|u-\langle u,v\rangle v/\|v\|^2\|^2$ gives

$$
\boxed{|\langle u,v\rangle|\leq\|u\|\|v\|.}
$$

The case $v=0$ is immediate. This [Cauchy-Schwarz inequality](../../../../cauchy-schwarz-inequality.md) shows that $f_v$ is bounded linear with [norm](../../../../norm.md) at most $\|v\|$. For $v\ne0$, evaluation at $v/\|v\|$ gives equality; for $v=0$ both norms vanish. The Banach dual is the space of all bounded linear functionals with the [operator norm](../../../../operator-norm.md).

The [Riesz representation theorem](../../../../riesz-representation-theorem.md) asserts that every $f\in V'$ is uniquely $f(u)=\langle u,v\rangle$ for some $v\in V$, with $\|f\|=\|v\|$. If $f=0$, take $v=0$. Otherwise put $W=\ker f$, a [closed subspace](../../../../closed-subspace.md), and use the projection theorem to obtain $w\in W^\perp$ with $f(w)=1$. Since $u-f(u)w\in W$, $\langle u,w\rangle=f(u)\|w\|^2$. Thus $v=w/\|w\|^2$ represents $f$. If two vectors represent it, their difference has [inner product](../../../../inner-product-split.md) zero with every vector, in particular itself, giving uniqueness. The [norm](../../../../norm.md) statement was already proved.

The space $P_n$ is finite-dimensional and hence [complete](../../../../completeness.md); evaluation at zero is bounded there by equivalence of finite-dimensional norms. Riesz therefore supplies exactly one $q_n\in P_n$. In any [orthonormal](../../../../orthonormal-set.md) [polynomial](../../../../polynomial-split.md) basis,

$$
\boxed{q_n(t)=\sum_{j=0}^n\overline{p_j(0)}p_j(t),\qquad\|q_n\|^2=\sum_{j=0}^n|p_j(0)|^2.}
$$

For the real Legendre functions the bars may be omitted.

**The printed even-degree normalization has an error.** [Orthogonality](../../../../orthogonal-vectors.md) forces a degree-two [polynomial](../../../../polynomial-split.md) to be a scalar multiple of $3t^2-1$, whose squared integral on $[-1,1]$ is $8/5$. Hence any [orthonormal](../../../../orthonormal-set.md) choice has $|p_2(0)|^2=5/8$, whereas the printed formula gives $3/8$. The factor under its square root must be $4m+1$ instead of $2m+1$. Signs of the individual polynomials can be chosen so that the values at zero are positive; these signs do not affect $q_n$ or its [norm](../../../../norm.md).

Put $M=\lfloor n/2\rfloor$ and $c_m=\binom{2m}{m}/4^m$. With the consistent [orthonormal](../../../../orthonormal-set.md) normalization the [norm](../../../../norm.md) is

$$
\boxed{\|q_n\|^2=\frac12\sum_{m=0}^M(4m+1)c_m^2=\frac{(2M+1)^2c_M^2}{2},\qquad\|q_n\|=\frac{(2M+1)c_M}{\sqrt2}.}
$$

The finite sum telescopes because $c_m=(2m-1)c_{m-1}/(2m)$, so $(2m+1)^2c_m^2-(2m-1)^2c_{m-1}^2=(4m+1)c_m^2$. If one substitutes the erroneous printed values formally instead, one obtains $\frac12\sum_{m=0}^M(2m+1)c_m^2$; that is not the [norm](../../../../norm.md) of the actual [orthonormal](../../../../orthonormal-set.md) Legendre evaluation representer.

For a [polynomial](../../../../polynomial-split.md) $r$ of degree $d$, the defining identity gives $\langle r,q_n\rangle=r(0)$ for every $n\geq d$, so the requested limit is eventually constant. It does **not** extend to all of $L^2$. First, evaluation at a point is not well-defined on equivalence classes. More strongly, the functional norms $\|q_n\|$ are unbounded. Indeed the largest binomial coefficient in row $2m$ is at least the average, so $c_m\geq1/(2m+1)$, and the displayed sum dominates a divergent constant multiple of the [harmonic series](../../../../harmonic-series.md). The [Uniform boundedness principle](../../../../uniform-boundedness-principle.md) then provides an $L^2$ function for which $\sup_n|\langle r,q_n\rangle|=\infty$. Thus no choice of point representative can restore the assertion for all $L^2$ functions.

## ↑ Ancestors (12)

1. [5](../5.md)
2. [B](../../b.md)
3. [2008](../../../2008-split.md)
4. [Past exam of the analysis course of the University of Oxford](../../../split.md)
5. [Analysis course of the University of Oxford](../../../../analysis-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
