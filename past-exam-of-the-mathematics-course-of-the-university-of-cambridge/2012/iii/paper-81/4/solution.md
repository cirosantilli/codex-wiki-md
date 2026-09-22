<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

We prove the [Dirichlet density](../../../../../dirichlet-density.md) form of the [Chebotarev density theorem](../../../../../chebotarev-density-theorem.md). Let $L/K$ be a finite [Galois extension](../../../../../finite-galois-extension.md) with [Galois group](../../../../../galois-group.md) $G$, let $C$ be a [conjugacy class](../../../../../conjugacy-class.md) in $G$, and let $S_C$ consist of the [unramified](../../../../../unramified-extension.md) prime ideals of $K$ whose [Frobenius conjugacy class](../../../../../frobenius-conjugacy-class.md) is $C$. The assertion is

$$
\boxed{\delta(S_C)=\lim_{s\downarrow1}
\frac{\displaystyle\sum_{\mathfrak p\in S_C}(N\mathfrak p)^{-s}}
{\log(1/(s-1))}=\frac{|C|}{|G|}.}
$$

The same result holds for any union of [conjugacy classes](../../../../../conjugacy-class.md), by addition. The following proof uses exactly the allowed one-dimensional [Artin L-function](../../../../../artin-l-function.md) behavior at $1$ and the permitted induction and Euler-product properties.

First determine the [order of vanishing](../../../../../order-of-vanishing.md) at $1$ for an arbitrary [character of a representation](../../../../../character-of-a-representation.md) $\chi$ of $G$. The [Brauer induction](../../../../../brauer-induction.md) theorem supplies subgroups $H_j\leq G$, [linear characters](../../../../../linear-character.md) $\psi_j$ of $H_j$, and integers $n_j$, possibly negative, such that

$$
\chi=\sum_jn_j\operatorname{Ind}_{H_j}^G\psi_j.
$$

Put $K_j=L^{H_j}$. Compatibility of [Artin L-functions](../../../../../artin-l-function.md) with [induced representations](../../../../../induced-representation.md) and direct sums gives, initially for $\operatorname{Re}s>1$,

$$
L_K(\chi,s)=\prod_jL_{K_j}(\psi_j,s)^{n_j}.
$$

Each $\psi_j$ is a one-dimensional [Galois representation](../../../../../galois-representation.md) for $L/K_j$, so the stated analytic assumptions apply to every factor. A trivial $\psi_j$ contributes a simple pole; a nontrivial $\psi_j$ is holomorphic and nonzero at one. Thus the product is meromorphic near one and

$$
\operatorname{ord}_{s=1}L_K(\chi,s)
=-\sum_jn_j\langle\psi_j,1_{H_j}\rangle_{H_j}.
$$

The [character inner product](../../../../../character-inner-product.md) is $\langle\alpha,\beta\rangle_G=|G|^{-1}\sum_{g\in G}\alpha(g)\overline{\beta(g)}$. Applying [Frobenius reciprocity](../../../../../frobenius-reciprocity.md) to each induced term gives

$$
\boxed{\operatorname{ord}_{s=1}L_K(\chi,s)
=-\sum_jn_j\langle\operatorname{Ind}_{H_j}^G\psi_j,1_G\rangle_G
=-\langle\chi,1_G\rangle_G.}
$$

In particular, a nontrivial [irreducible character](../../../../../irreducible-character.md) has order zero, so its [Artin L-function](../../../../../artin-l-function.md) is holomorphic and nonzero near one. For the trivial character, $L_K(1_G,s)=\zeta_K(s)$, the [Dedekind zeta function](../../../../../dedekind-zeta-function.md) of the base field $K$, and its pole is simple. This argument establishes the behavior needed at one, not holomorphy everywhere for arbitrary [Artin L-functions](../../../../../artin-l-function.md).

Next convert that order calculation into a prime sum. For an [irreducible character](../../../../../irreducible-character.md) $\chi$, choose a unitary representation of dimension $d_\chi$ affording it, and choose a [Frobenius automorphism](../../../../../frobenius-automorphism.md) $g_{\mathfrak p}$ at each [unramified](../../../../../unramified-extension.md) prime. The logarithm specified by the absolutely convergent [Euler product](../../../../../euler-product.md) gives, for real $s>1$,

$$
\log L_K(\chi,s)
=\sum_{\mathfrak p\ \mathrm{unramified}}\sum_{m\geq1}
\frac{\chi(g_{\mathfrak p}^{\,m})}{m(N\mathfrak p)^{ms}}
+R_\chi(s).
$$

Only finitely many ramified primes occur. Their Euler-factor logarithms $R_\chi(s)$ stay bounded near one, since the relevant eigenvalues have modulus one and $(N\mathfrak p)^{-1}<1$. Also $|\chi(g)|\leq d_\chi$, so the contribution with $m\geq2$ is uniformly bounded for $s\geq1$ by

$$
\sum_{\mathfrak p}\sum_{m\geq2}
\frac{d_\chi}{m(N\mathfrak p)^{ms}}
\leq2d_\chi\sum_{\mathfrak p}(N\mathfrak p)^{-2}<\infty.
$$

Convergence follows, for example, from the convergent ideal series defining $\zeta_K(2)$. Therefore

$$
\sum_{\mathfrak p\ \mathrm{unramified}}
\frac{\chi(g_{\mathfrak p})}{(N\mathfrak p)^s}
=\log L_K(\chi,s)+O(1).
$$

Writing $a_\chi=\langle\chi,1_G\rangle_G$, the order computation means $L_K(\chi,s)=(s-1)^{-a_\chi}U_\chi(s)$, where $U_\chi$ is holomorphic and nonzero near one. Choose its local logarithm. Along the real interval approaching one, this and the Euler-product logarithm differ only by a fixed multiple of $2\pi i$. Consequently

$$
\boxed{\sum_{\mathfrak p\ \mathrm{unramified}}
\frac{\chi(g_{\mathfrak p})}{(N\mathfrak p)^s}
=a_\chi\log\frac1{s-1}+O(1).}
$$

Only the trivial [irreducible character](../../../../../irreducible-character.md) has $a_\chi=1$; all the others have $a_\chi=0$.

Finally, [character orthogonality](../../../../../character-orthogonality.md) makes the [irreducible characters](../../../../../irreducible-character.md) an orthonormal basis of class functions. For $c\in C$, the coefficient of $\chi$ in the class indicator is $\langle1_C,\chi\rangle_G=(|C|/|G|)\overline{\chi(c)}$. Hence

$$
1_C(g)=\frac{|C|}{|G|}\sum_{\chi\in\operatorname{Irr}(G)}
\overline{\chi(c)}\chi(g).
$$

Sum this identity over the [unramified](../../../../../unramified-extension.md) primes with weight $(N\mathfrak p)^{-s}$. The finite character sum and the boxed estimates give

$$
\boxed{\sum_{\mathfrak p\in S_C}(N\mathfrak p)^{-s}
=\frac{|C|}{|G|}\log\frac1{s-1}+O(1).}
$$

Dividing by $\log(1/(s-1))$ proves the asserted [Dirichlet density](../../../../../dirichlet-density.md). The same Euler-product calculation with $\zeta_K$ gives $\sum_{\mathfrak p}(N\mathfrak p)^{-s}=\log(1/(s-1))+O(1)$, so using all primes as the denominator is equivalent. Finitely many ramified primes do not affect either limit. No prime-counting asymptotic or natural-density Tauberian step is required by this proof.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 81](../../paper-81-split.md)
3. [Iii](../../split.md)
4. [2012](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
