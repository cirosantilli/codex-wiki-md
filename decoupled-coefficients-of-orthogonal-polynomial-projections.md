# Decoupled coefficients of orthogonal polynomial projections

↑ **Parent:** [Orthogonal polynomial](orthogonal-polynomial-split.md)

Let $f$ be a real [function](function-split.md) with $\|f\|_w^2=\int_a^b f(x)^2w(x)\,dx<\infty$, and let $V_m$ be the [vector space](vector-space-split.md) of real [polynomials](polynomial-split.md) of degree at most $m$. Its [orthogonal projection](orthogonal-projection.md) is the [least-squares polynomial in an orthogonal-polynomial basis](least-squares-polynomial-in-an-orthogonal-polynomial-basis.md)

$$
q_m=\sum_{n=0}^m c_np_n,\qquad c_n=\frac{\langle f,p_n\rangle_w}{h_n},\qquad h_n=\langle p_n,p_n\rangle_w.
$$

Each [coefficient](coefficient.md) depends on just one [weighted inner product](weighted-inner-product.md) with $f$ and one squared [norm](norm.md). In particular, the [coefficients](coefficient.md) $c_0,\ldots,c_m$ stay the same when the allowed [polynomial degree](degree-of-a-polynomial.md) increases. This statement assumes a fixed weight, interval and normalization of the [orthogonal polynomials](orthogonal-polynomial-split.md).

To see why the [least-squares normal equations](normal-equations-for-linear-least-squares.md) decouple, first write a trial [polynomial](polynomial-split.md) as $q=\sum_{j=0}^m a_j\phi_j$ in any [basis](basis.md) of $V_m$. The residual must be [orthogonal](orthogonal-vectors.md) to each permitted direction, giving

$$
\sum_{j=0}^m G_{ij}a_j=b_i,\qquad G_{ij}=\langle\phi_j,\phi_i\rangle_w,\qquad b_i=\langle f,\phi_i\rangle_w.
$$

The [Gram matrix](gram-matrix.md) usually couples the unknown [coefficients](coefficient.md). With $\phi_j=p_j$, it becomes $G_{ij}=h_i\delta_{ij}$, leaving the separate equations $h_i a_i=b_i$. For the [monomial basis](monomial-basis.md) on $[-1,1]$ with $w=1$, by contrast, $G_{ij}$ is zero when $i+j$ is odd and $2/(i+j+1)$ when $i+j$ is even. Distinct even powers, or distinct odd powers, remain coupled.

There is also a proof of the minimum that uses no [differentiation](differentiation.md). The defining [coefficients](coefficient.md) give $\langle f-q_m,p_n\rangle_w=0$ for $0\leq n\leq m$. Thus $f-q_m$ is [orthogonal](orthogonal-vectors.md) to all of $V_m$. For every $v\in V_m$, the [Pythagorean theorem in an inner-product space](pythagorean-theorem-in-an-inner-product-space.md) gives

$$
\|f-v\|_w^2=\|f-q_m\|_w^2+\|q_m-v\|_w^2.
$$

The second term is nonnegative and vanishes exactly when $v=q_m$, proving that the [least-squares solution](least-squares-solution-of-a-linear-inverse-problem.md) is unique. This is an integrated squared-error optimum; it does not assert a smallest error at every point or a smallest [uniform norm](supremum-norm.md).

For $N>m$, the nested [orthogonal projections](orthogonal-projection.md) satisfy the exact residual budget

$$
\|f-q_m\|_w^2=\|f-q_N\|_w^2+\sum_{n=m+1}^{N}c_n^2h_n.
$$

Indeed, $q_N-q_m$ is a [linear combination](linear-combination.md) of mutually [orthogonal polynomials](orthogonal-polynomial-split.md), and $f-q_N$ is [orthogonal](orthogonal-vectors.md) to it. Every newly retained component removes exactly $c_n^2h_n$ from the squared error. No infinite expansion or completeness assumption is needed for this finite identity. The [Legendre least-squares projections of a cubic](legendre-least-squares-projections-of-a-cubic.md) make every term explicit.

**Table of contents**

- [Legendre least-squares projections of a cubic](legendre-least-squares-projections-of-a-cubic.md)

## ↑ Ancestors (6)

1. [Orthogonal polynomial](orthogonal-polynomial-split.md)
2. [Numerical analysis](numerical-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Orthogonal polynomial](orthogonal-polynomial-split.md)
