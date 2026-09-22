<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

The ordinary interpolation formulation is unambiguous for strictly increasing knots; repeated knots require specified confluent interpolation or a limiting convention. First take distinct knots and $k\ge2$, and for fixed $t$ write $F_t(u)=(u-t)_+^{k-1}$. The two degree-at-most-$k-1$ [Lagrange interpolation polynomials](../../../../../lagrange-polynomial.md) $\ell_i(\cdot,t)$ and $\ell_{i+1}(\cdot,t)$ agree at the $k-1$ shared knots $t_{i+1},\ldots,t_{i+k-1}$. Their difference is therefore

$$
\ell_{i+1}(x,t)-\ell_i(x,t)=c_i(t)\prod_{r=1}^{k-1}(x-t_{i+r})=c_i(t)\omega_i(x).
$$

This remains valid if their difference has lower degree: the [coefficient](../../../../../coefficient.md) is then zero. The [leading coefficient](../../../../../leading-coefficient-of-a-polynomial.md) of a degree-at-most-$k-1$ interpolant is its order-$(k-1)$ [divided difference](../../../../../divided-difference.md). Comparing leading [coefficients](../../../../../coefficient.md) and using the divided-difference recursion gives

$$
\begin{aligned}
c_i(t)&=[t_{i+1},\ldots,t_{i+k}]F_t-[t_i,\ldots,t_{i+k-1}]F_t\\
&=(t_{i+k}-t_i)[t_i,\ldots,t_{i+k}]F_t=N_i(t).
\end{aligned}
$$

Consequently the [Lee interpolation identity](../../../../../lee-interpolation-identity.md) holds for every real $x,t$:

$$
\boxed{\omega_i(x)N_i(t)=\ell_{i+1}(x,t)-\ell_i(x,t).}
$$

No differentiability of the truncated power in its argument was needed for this distinct-node proof.

Sum the identity over $i=1,\ldots,n$. The right side telescopes, giving $\sum_i\omega_i(x)N_i(t)=\ell_{n+1}(x,t)-\ell_1(x,t)$. When $t_k<t<t_{n+1}$, all the nodes for $\ell_1$ lie below $t$, so its interpolation data are zero and $\ell_1\equiv0$. All the nodes for $\ell_{n+1}$ lie above $t$, where $F_t(u)=(u-t)^{k-1}$ is already a [polynomial](../../../../../polynomial-split.md) of the admissible degree. Uniqueness of [polynomial](../../../../../polynomial-split.md) interpolation gives $\ell_{n+1}(x,t)=(x-t)^{k-1}$. Therefore the [Marsden identity](../../../../../marsden-identity.md) is

$$
\boxed{(x-t)^{k-1}=\sum_{i=1}^n\omega_i(x)N_i(t),\qquad t_k<t<t_{n+1},\quad x\in\mathbb R.}
$$

For order one the empty product is one, the interpolants are constants and a consistent half-open interval convention for $(u-t)_+^0$ gives the same telescoping proof. Nondecreasing repeated-knot sequences can be treated by the appropriate confluent or limiting convention wherever that definition is valid; merely specifying repeated data values does not uniquely determine the interpolation [polynomials](../../../../../polynomial-split.md). The basic open knot interval in the [Marsden identity](../../../../../marsden-identity.md) avoids endpoint convention ambiguity.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 61](../../paper-61-split.md)
3. [Iii](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
