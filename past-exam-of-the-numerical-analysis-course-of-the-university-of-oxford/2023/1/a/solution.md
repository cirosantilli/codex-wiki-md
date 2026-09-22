<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For a complex $n\times n$ [matrix](../../../../matrix.md) $B=(b_{ij})$, put

$$
R_i=\sum_{j\ne i}|b_{ij}|,\qquad
D_i=\{z\in\mathbb C:|z-b_{ii}|\leq R_i\}.
$$

The [Gershgorin circle theorem](../../../../gershgorin-circle-theorem.md) states that

$$
\boxed{\operatorname{spec}(B)\subseteq\bigcup_{i=1}^nD_i.}
$$

To prove it, let $Bv=\lambda v$ with $v\ne0$, and choose $i$ for which $|v_i|=\max_j|v_j|>0$. The $i$th coordinate of the [eigenvalue equation](../../../../eigenvalue-equation.md) gives

$$
(\lambda-b_{ii})v_i=\sum_{j\ne i}b_{ij}v_j.
$$

The [triangle inequality](../../../../triangle-inequality.md), followed by division by $|v_i|$, gives

$$
|\lambda-b_{ii}|\leq\sum_{j\ne i}|b_{ij}|\frac{|v_j|}{|v_i|}
\leq\sum_{j\ne i}|b_{ij}|=R_i.
$$

Thus $\lambda\in D_i$, proving the assertion for every [eigenvalue](../../../../eigenvalue.md).

The second theorem, [Gershgorin eigenvalue counting](../../../../gershgorin-eigenvalue-counting.md), says that if a union of $k$ indexed [Gershgorin discs](../../../../gershgorin-disc.md) is disjoint from the remaining $n-k$ [Gershgorin discs](../../../../gershgorin-disc.md), that union contains exactly $k$ [eigenvalues](../../../../eigenvalue.md), counted with [algebraic multiplicity](../../../../algebraic-multiplicity.md). In particular,

$$
\boxed{\text{An isolated Gershgorin disc contains exactly one simple eigenvalue.}}
$$

Discs that touch are not disjoint; overlapping [Gershgorin discs](../../../../gershgorin-disc.md) cannot individually be assigned one [eigenvalue](../../../../eigenvalue.md) each.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the numerical analysis course of the University of Oxford](../../../split.md)
5. [Numerical analysis course of the University of Oxford](../../../../numerical-analysis-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
