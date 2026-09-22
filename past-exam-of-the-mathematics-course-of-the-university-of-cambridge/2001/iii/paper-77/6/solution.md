<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

In $N$ variables, pad $\lambda$ to length $N$ and set $\delta=(N-1,N-2,\ldots,0)$. Define the [alternant](../../../../../monomial-alternant.md)

$$
a_\gamma(x)=\det[x_j^{\gamma_i}]_{i,j=1}^N,
\qquad a_\delta=\prod_{i<j}(x_i-x_j).
$$

The last equality is the [Vandermonde determinant](../../../../../vandermonde-determinant.md) with the indicated descending-exponent convention.

We use the [Jacobi–Trudi identity](../../../../../jacobi-trudi-identity.md) proved above and give the [determinant](../../../../../determinant.md) step explicitly. Let

$$
J_{ij}=h_{\lambda_i-i+j}(X),\qquad
B_{jk}=(-1)^{N-j}e_{N-j}(X\setminus x_k).
$$

Put $b_i=\lambda_i+N-i\ge0$. The generating-function identity

$$
H_X(t)\prod_{r\ne k}(1-x_rt)=\frac1{1-x_kt}
$$

shows, by extracting the coefficient of $t^{b_i}$, that

$$
(JB)_{ik}
=\sum_{j=1}^N h_{b_i-N+j}(X)(-1)^{N-j}
e_{N-j}(X\setminus x_k)=x_k^{b_i}.
$$

When $\lambda$ is empty, $J_{ij}=h_{-i+j}$ is upper triangular with diagonal one, and the product [matrix](../../../../../matrix.md) is $[x_k^{N-i}]$. Thus $\det B=a_\delta$. Taking [determinants](../../../../../determinant.md) for general $\lambda$ gives $s_\lambda a_\delta=a_{\lambda+\delta}$ and proves the [bialternant formula](../../../../../bialternant-formula.md)

$$
\boxed{s_\lambda(x_1,\ldots,x_N)=\frac{a_{\lambda+\delta}}{a_\delta}.}
$$

The equality before division is [polynomial](../../../../../polynomial-split.md). Consequently the quotient extends at coincident variables as the [Schur polynomial](../../../../../schur-polynomial.md).

For the Fourier minors, choose a square submatrix of size $d\le p$, with distinct row residues $r_1,\ldots,r_d$ and column residues. Sort the columns into decreasing exponents $b_1>\cdots>b_d$ in $\{0,\ldots,p-1\}$; this changes a [determinant](../../../../../determinant.md) only by sign. Put

$$
\lambda_i=b_i-(d-i).
$$

Because the $b_i$ are distinct nonnegative integers, $b_i\ge d-i$, and $b_i-b_{i+1}\ge1$. Hence $\lambda$ is a partition. With $x_j=\zeta^{r_j}$, [transposition](../../../../../transposition-permutation.md) of the submatrix and the [bialternant formula](../../../../../bialternant-formula.md) give

$$
\det B=\pm a_b(x)
=\pm a_\delta(x)s_\lambda(x),\qquad \delta=(d-1,\ldots,0).
$$

The $x_j$ are distinct, so the Vandermonde factor does not vanish.

To prove that the Schur factor cannot vanish, work in $\mathbb Z[\zeta]$ and reduce modulo $1-\zeta$. Since the prime cyclotomic [polynomial](../../../../../polynomial-split.md) is $\Phi_p(t)=1+t+\cdots+t^{p-1}$ and $\Phi_p(1)=p$,

$$
\mathbb Z[\zeta]/(1-\zeta)\cong\mathbb F_p.
$$

All $x_j$ reduce to one, and the Schur factor reduces to $s_\lambda(1^d)$. We need its value, not an assumption that the specialization is nonzero. The [Schur evaluation at all ones](../../../../../schur-evaluation-at-all-ones.md) formula is

$$
s_\lambda(1^d)=
\prod_{i<j}\frac{b_i-b_j}{j-i}.
$$

For completeness, substitute $x_j=e^{ty_j}$ with distinct $y_j$ into the bialternant. In the exponential expansions, the first nonzero [determinant](../../../../../determinant.md) coefficient uses exactly the distinct powers $0,1,\ldots,d-1$ and has degree $d(d-1)/2$ in $t$. The [determinant](../../../../../determinant.md) in the $y_j$ and the factorial factors are common to numerator and denominator. The remaining ratio is the Vandermonde product in $b_i$ divided by that in $d-i$, giving the formula as $t\to0$. Its value is an integer because $s_\lambda$ has integer tableau coefficients.

Every positive difference $b_i-b_j$ and $j-i$ is strictly less than $p$. Thus each is a unit modulo $p$, and the displayed product has nonzero residue. A zero Schur factor would have zero residue, a contradiction. This proves the [prime Fourier matrix minor theorem](../../../../../prime-fourier-matrix-minor-theorem.md):

$$
\boxed{\text{Every square minor of }[\zeta^{jk}]_{j,k=0}^{p-1}\text{ is nonzero}.}
$$

Finally use the one-row shape $\lambda=(r)$, for which $s_{(r)}=h_r$. Its numerator [determinant](../../../../../determinant.md) has first-row exponents $N-1+r$ and subsequent exponents $N-2,\ldots,0$. Expanding along the first row gives cofactors equal, up to their signs, to the [Vandermonde determinant](../../../../../vandermonde-determinant.md) in all variables except $x_k$. Since

$$
\frac{a_\delta(X)}{a_\delta(X\setminus x_k)}
=(-1)^{k-1}\prod_{i\ne k}(x_k-x_i),
$$

the cofactor sign $(-1)^{1+k}$ cancels the indicated sign in the quotient. Therefore

$$
\boxed{h_r(x_1,\ldots,x_N)=
\sum_{k=1}^N x_k^{N-1+r}\prod_{i\ne k}(x_k-x_i)^{-1}.}
$$

This rational expression is first computed for pairwise distinct variables; its sum is the [polynomial](../../../../../polynomial-split.md) $h_r$, giving the continuous [polynomial](../../../../../polynomial-split.md) extension when variables coincide.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 77](../../paper-77-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
