<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

Use the induction product of symmetric-group [characters](../../../../../character-of-a-representation.md): for $a\ge0$, $[a]$ is the trivial [character](../../../../../character-of-a-representation.md) of $S_a$, $[0]$ is the unit and $[a]=0$ for $a<0$. Products mean induction of external [tensor products](../../../../../tensor-product.md). The determinantal form is

$$
\boxed{[\lambda]=\det\bigl([\lambda_i-i+j]\bigr)_{1\le i,j\le r},}
$$

where $r\ge\ell(\lambda)$. Each [determinant](../../../../../determinant.md) term is a virtual [character](../../../../../character-of-a-representation.md) of $S_n$, because its indices sum to $n$.

Here is a proof. The [Frobenius characteristic map](../../../../../frobenius-characteristic-map.md) sends $[a]$ to the [complete homogeneous symmetric function](../../../../../complete-homogeneous-symmetric-polynomial.md) $h_a$, and induction products to multiplication. By [Young's rule](../../../../../young-s-rule.md) its value on $[\lambda]$ is the [Schur function](../../../../../schur-polynomial.md) $s_\lambda$, the generating function of [semistandard tableaux](../../../../../semistandard-young-tableau.md) of shape $\lambda$. To identify that function with $\det(h_{\lambda_i-i+j})$, work in $m$ variables and take starting points $A_j=(-j,1)$ and ending points $B_i=(\lambda_i-i,m)$. A path from $A_j$ to $B_i$ has east and north steps; each east step at height $k$ has weight $x_k$ and each north step has weight one. Its east-step count is $\lambda_i-i+j$, so its weight sum is $h_{\lambda_i-i+j}$. Expanding the [determinant](../../../../../determinant.md) sums signed systems of paths with permuted endpoints. For a system with an intersection, exchange the two tails after the first intersection. This preserves its monomial weight and reverses the endpoint [permutation](../../../../../permutation.md)'s sign, so all intersecting systems cancel in pairs. Nonintersecting systems necessarily have the identity endpoint [permutation](../../../../../permutation.md) and correspond precisely to weak rows with strictly increasing columns, namely [semistandard tableaux](../../../../../semistandard-young-tableau.md) of shape $\lambda$. Their signs are positive. This proves $s_\lambda=\det(h_{\lambda_i-i+j})$, the [Jacobi–Trudi identity](../../../../../jacobi-trudi-identity.md), and injectivity of the [Frobenius characteristic map](../../../../../frobenius-characteristic-map.md) gives the [character](../../../../../character-of-a-representation.md) formula above. The path sum may be taken in finitely many variables first and then stabilized, so no infinite formal sum is required in the argument.

A removable [rim hook](../../../../../rim-hook.md), or border strip, of length $k$ is a connected skew diagram $\lambda/\nu$ of $k$ cells with no $2\times2$ square, where removal leaves a [partition of an integer](../../../../../partition-of-an-integer.md). Its leg length is the number of occupied rows minus one. The [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md) states

$$
\boxed{\chi^\lambda(k,\rho)=\sum_{\nu:\lambda/\nu\text{ is a }k\text{-rim hook}}
(-1)^{\operatorname{leg}(\lambda/\nu)}\chi^\nu(\rho).}
$$

A proof sketch follows directly from the alternant form of [Schur functions](../../../../../schur-polynomial.md). Multiply an alternant by $p_k=\sum_jx_j^k$. In each term one alternant exponent increases by $k$. Equal exponents cancel; otherwise reordering the exponents contributes the sign of the number crossed. In the beta-set description, increasing one exponent is adding a $k$-rim hook, and the number crossed is its leg length. Therefore $p_ks_\nu=\sum_\lambda(-1)^{\operatorname{leg}(\lambda/\nu)}s_\lambda$. Taking its adjoint in the [Hall inner product of symmetric functions](../../../../../hall-inner-product-of-symmetric-functions.md), where [Schur functions](../../../../../schur-polynomial.md) are orthonormal and [power-sum symmetric polynomials](../../../../../power-sum-symmetric-polynomial.md) have squared norm $z_\rho$, reads off the value at a $k$-cycle and the remaining [cycle type](../../../../../cycle-type.md). This gives the stated rule and explains its sign.

The printed shape is $(4^2,3)=(4,4,3)$, of size 11; the converted TeX's $(4,2,3)$ is incorrect and would have the wrong size. There are two removable length-5 [rim hooks](../../../../../rim-hook.md). They leave $(3,2,1)$ with leg length 2 and $(4,2)$ with leg length 1. Thus

$$
\chi^{(4,4,3)}(5,4,2)=\chi^{(3,2,1)}(4,2)-\chi^{(4,2)}(4,2).
$$

The staircase $(3,2,1)$ has no removable length-4 [rim hook](../../../../../rim-hook.md), so its term is zero. The unique removable length-4 [rim hook](../../../../../rim-hook.md) of $(4,2)$ leaves $(1,1)$ and has leg length 1. The remaining length-2 [rim hook](../../../../../rim-hook.md) in $(1,1)$ also has leg length 1, giving $\chi^{(4,2)}(4,2)=(-1)(-1)=1$. Hence

$$
\boxed{\chi^{(4,4,3)}(5,4,2)=-1.}
$$

As a separate [determinant](../../../../../determinant.md) check, the only term whose row sizes can be unions of cycles of lengths $5,4,2$ is the [transposition](../../../../../transposition-permutation.md) term with sizes $(4,5,2)$. Its [permutation character](../../../../../permutation-character.md) has value one and its [determinant](../../../../../determinant.md) sign is negative.

Taking $k=1$ in the [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md) removes a single corner and every leg length is zero. Evaluating on a [permutation](../../../../../permutation.md) fixing the distinguished point therefore gives

$$
\operatorname{Res}^{S_n}_{S_{n-1}}\chi^\lambda=\sum_{\nu\in\lambda^-}\chi^\nu.
$$

This is the [restriction branching rule for a symmetric group](../../../../../restriction-branching-rule-for-a-symmetric-group.md); ordinary [semisimple representation](../../../../../semisimple-representation.md) theory converts the [character](../../../../../character-of-a-representation.md) equality into a direct-sum decomposition. [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) gives the corresponding add-one-cell induction rule.

For a positive prime $p$, the [weight of a partition](../../../../../weight-of-a-partition.md) $\lambda$ at prime modulus $p$, denoted $w$, is the number of length-$p$ [rim hooks](../../../../../rim-hook.md) removed in reaching its [partition core](../../../../../core-of-a-partition.md) $\kappa$, so $n=|\kappa|+pw$. On a prime-modulus [partition abacus](../../../../../abacus-of-a-partition.md) write its [partition quotient](../../../../../quotient-of-a-partition.md) as $(\lambda^{(0)},\ldots,\lambda^{(p-1)})$ and put $w_i=|\lambda^{(i)}|$, with $\sum_iw_i=w$. Removing a length-$p$ [rim hook](../../../../../rim-hook.md) removes one corner from one quotient [partition of an integer](../../../../../partition-of-an-integer.md). Complete removal sequences therefore number

$$
N_p(\lambda)=\binom{w}{w_0,\ldots,w_{p-1}}\prod_{i=0}^{p-1}f^{\lambda^{(i)}}
=\frac{w!}{\prod_iH_{\lambda^{(i)}}},
$$

where $H_\alpha$ is the [hook product of a partition](../../../../../hook-product-of-a-partition.md) and $H_\varnothing=1$. Each component's [standard tableaux](../../../../../standard-young-tableau.md) encode its possible removal orders, and the multinomial coefficient interleaves the components.

All these sequences have the same total sign $\varepsilon_p(\lambda)$. To see this, label the beads on each runner in their preserved order. Each slide crosses exactly the beads counted by its rim-hook leg. Its sign is the change in the total order of bead labels, and the product telescopes to the [permutation](../../../../../permutation.md) from the initial ordering to the final packed-core ordering, independently of the slides chosen. Repeating the [Murnaghan–Nakayama rule](../../../../../murnaghan-nakayama-rule.md) on the $w$ distinguished $p$-cycles gives

$$
\boxed{\chi^\lambda(\pi\rho)=\varepsilon_p(\lambda)N_p(\lambda)\chi^\kappa(\pi).}
$$

Here $\pi$ acts on the complementary $n-pw$ letters; no $p$-regularity hypothesis on $\pi$ is necessary. If its [cycle type](../../../../../cycle-type.md) contains a part divisible by $p$, the [partition core](../../../../../core-of-a-partition.md) [character](../../../../../character-of-a-representation.md) is zero, since its [partition abacus](../../../../../abacus-of-a-partition.md) admits no hook removal of a length divisible by $p$. For $w=0$ the coefficient and sign are one.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 4](../../paper-4-split.md)
3. [Iii](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
