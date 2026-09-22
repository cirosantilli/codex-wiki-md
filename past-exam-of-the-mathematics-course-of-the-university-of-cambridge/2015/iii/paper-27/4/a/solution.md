<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $\mathbf1(n)=1$ and $\epsilon(n)=1_{n=1}$, the identity for [Dirichlet convolution](../../../../../../dirichlet-convolution.md). The elementary identities needed are

$$
\mu*\mathbf1=\epsilon,\qquad\Lambda*\mathbf1=\log,\qquad\mu*\log=\Lambda.
$$

For the first, [prime factorization](../../../../../../fundamental-theorem-of-arithmetic.md) gives $\sum_{d\mid n}\mu(d)=\prod_{p\mid n}(1-1)$ when $n>1$, and one when $n=1$. For the second, if $n=\prod p^{a_p}$, then $\sum_{d\mid n}\Lambda(d)=\sum_pa_p\log p=\log n$, the [Von Mangoldt divisor identity](../../../../../../von-mangoldt-divisor-identity.md). Convolving the second identity with $\mu$ proves the third.

For $U,V\geq1$, let the subscripts $\leq U$, $>U$, $\leq V$, $>V$ denote truncations. The [Vaughan identity](../../../../../../vaughan-s-identity.md) is

$$
\boxed{\Lambda=\Lambda_{\leq V}+\mu_{\leq U}*\log-\mu_{\leq U}*\mathbf1*\Lambda_{\leq V}+\mu_{>U}*\mathbf1*\Lambda_{>V}.}
$$

Its pointwise form is

$$
\Lambda(n)=\Lambda(n)1_{n\leq V}
+\sum_{\substack{d\mid n\\d\leq U}}\mu(d)\log(n/d)
-\sum_{\substack{dc\mid n\\d\leq U,\ c\leq V}}\mu(d)\Lambda(c)
+\sum_{\substack{dcm=n\\d>U,\ c>V}}\mu(d)\Lambda(c).
$$

To prove it, use $\mu_{>U}*\mathbf1=\epsilon-\mu_{\leq U}*\mathbf1$ and $\mathbf1*\Lambda_{>V}=\log-\mathbf1*\Lambda_{\leq V}$. This gives

$$
\mu_{>U}*\mathbf1*\Lambda_{>V}
=\Lambda_{>V}-\mu_{\leq U}*\log+\mu_{\leq U}*\mathbf1*\Lambda_{\leq V},
$$

and rearrangement proves the formula, as in the [Vaughan identity proof](../../../../../../vaughan-identity-proof.md).

The [Bombieri–Vinogradov theorem](../../../../../../bombieri-vinogradov-theorem.md) states that for every $A>0$ there is $B>0$ such that

$$
\sum_{q\leq Q}\max_{(a,q)=1}\max_{2\leq y\leq x}\left|\psi(y;q,a)-\frac y{\phi(q)}\right|\ll_A\frac{x}{\log^Ax},\qquad Q\leq\frac{x^{1/2}}{\log^Bx}.
$$

Here $\psi(y;q,a)=\sum_{\substack{n\leq y\\n\equiv a\pmod q}}\Lambda(n)$ is the [Chebyshev function in an arithmetic progression](../../../../../../chebyshev-function-in-an-arithmetic-progression.md), and $\phi$ is the [Euler totient function](../../../../../../euler-totient-function.md). In particular, [partial summation](../../../../../../abel-s-summation-formula.md) gives

$$
\sum_{q\leq Q}\max_{(a,q)=1}\left|\pi(x;q,a)-\frac{\operatorname{Li}(x)}{\phi(q)}\right|\ll_A\frac{x}{\log^Ax},\qquad\operatorname{Li}(x)=\int_2^x\frac{dt}{\log t},
$$

after choosing the logarithmic saving in the weighted theorem sufficiently large and absorbing the [prime power](../../../../../../prime-power.md) terms. This is the offset [logarithmic integral function](../../../../../../logarithmic-integral-function.md).

For the proof strategy, [Orthogonality of Dirichlet characters](../../../../../../orthogonality-of-dirichlet-characters.md) converts errors in [arithmetic progressions](../../../../../../arithmetic-progression.md) into [character sums of Dirichlet characters](../../../../../../character-sum-of-a-dirichlet-character.md) weighted by $\Lambda$. Reduction to [primitive Dirichlet characters](../../../../../../primitive-dirichlet-character.md) is followed by the [character large sieve](../../../../../../character-large-sieve.md), which bounds their mean square by $O((N+Q^2)\sum|a_n|^2)$ with the usual $q/\phi(q)$ weights. The [Vaughan identity](../../../../../../vaughan-s-identity.md) separates the weighted sums into short terms, [Type I sums](../../../../../../type-i-sum.md) and [Type II sums](../../../../../../type-ii-sum.md). Direct inner-sum estimates handle the [Type I sums](../../../../../../type-i-sum.md); the [Cauchy-Schwarz inequality](../../../../../../cauchy-schwarz-inequality.md) and the [large sieve](../../../../../../large-sieve.md) control the [Type II sums](../../../../../../type-ii-sum.md). The [Siegel–Walfisz theorem](../../../../../../siegel-walfisz-theorem.md) supplies arbitrarily strong logarithmic savings for small moduli, where an average estimate alone would not suffice. A [dyadic decomposition](../../../../../../dyadic-decomposition.md), suitable $U,V$ and a sufficiently large $B$ absorb the divisor and logarithmic losses. This explains why the range is essentially $Q^2\leq x$, with logarithmic room to spare.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 27](../../../paper-27-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
