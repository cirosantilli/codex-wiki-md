<h1 id="40e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $A_h$ be the symmetric Dirichlet second-difference matrix. Its [eigenvalues](../../../../../../eigenvalue.md) are nonpositive, so every eigenvalue of

$$
R_h=(I-kA_h/2)^{-1}(I+kA_h/2)
$$

has modulus at most one. Thus $\|R_h\|_{2,h}\leq1$.

Insert the exact smooth solution into the scheme. The [local truncation error](../../../../../../local-truncation-error.md) per step has discrete norm $O(k^3+kh^2)$, from the order-three trapezoidal time residual and the order-two centred spatial residual. If $e^n$ is the grid error, stability and iteration give

$$
\|e^{n+1}\|_{2,h}\leq\|e^n\|_{2,h}+C(k^3+kh^2).
$$

There are at most $1/k$ steps and $e^0=0$, hence

$$
\max_n\|e^n\|_{2,h}\leq C(k^2+h^2)\to0.
$$

This proves convergence for every $μ=k/h^2>0$ without invoking the Lax equivalence theorem.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [40E](../../40e.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
