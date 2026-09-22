<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

The [Vandermonde determinant](../../../../../vandermonde-determinant.md) is

$$
\boxed{\det V(x_0,\ldots,x_{r-1})=\prod_{0\leq i<j<r}(x_j-x_i)}.
$$

Indeed, the [determinant](../../../../../determinant.md) is an alternating [polynomial](../../../../../polynomial-split.md), hence divisible by every $x_j-x_i$. Both sides have degree $r(r-1)/2$, and comparison of the coefficient of $x_0^0x_1^1\cdots x_{r-1}^{r-1}$ gives constant one. This is an identity over the integers, so reducing its coefficients modulo a [prime number](../../../../../prime-number.md) preserves it. For $r>p$, two residues coincide and the determinant vanishes. For $r=p$, choose all elements of $\mathbb F_p$ once to obtain a nonzero determinant.

For the ordering $0,1,\ldots,p-1$, this determinant is $D=\prod_{j=1}^{p-1}j!$. If $p$ is odd, put $h=(p-1)/2$. [Wilson theorem](../../../../../wilson-s-theorem.md) gives $j!(p-1-j)!=(-1)^{j+1}$. Pairing the factors with indices $j=0,\ldots,h-1$ and $p-1-j$, and leaving $h!$ unpaired, gives

$$
D=(-1)^{h(h+1)/2}h!.
$$

Every distinct ordering changes the determinant by its [permutation sign](../../../../../sign-of-a-permutation.md); repeated residues give zero. Thus **the possible values are $0,\pm h!$ for odd $p$, and $0,1$ for $p=2$.**

Use [Shamir's secret sharing](../../../../../shamir-s-secret-sharing.md): choose independent uniform $a_1,\ldots,a_{r-1}\in\mathbb F_p$, and engrave the shares $(x_i,P(x_i))$, where $P(X)=N+\sum_{j=1}^{r-1}a_jX^j$ and the $x_i$ are distinct nonzero field elements. We may take $p>n$; otherwise use a sufficiently large [finite field](../../../../../finite-field.md) extension and an agreed integer encoding. Any $r$ shares determine $P$ by [polynomial interpolation](../../../../../polynomial-interpolation.md) and hence $N=P(0)$. Given any $r-1$ shares and any proposed $N$, their equations in the coefficients have a unique solution: the coefficient matrix has determinant $\prod_i x_i$ times a nonzero [Vandermonde determinant](../../../../../vandermonde-determinant.md). Since the coefficients were uniform, the observed shares have the same distribution for every $N$. Thus they give no information about the secret.

For the fake, reduce its integers to field elements and first check that its abscissa is distinct and nonzero. Random collisions or a zero abscissa are immediately detectable and have probability $O(n/p)$; the following conclusions concern the overwhelmingly likely distinct-abscissa case.

With $r$ shares, there is always a unique degree-at-most-$r-1$ interpolating [polynomial](../../../../../polynomial-split.md). If all shares are genuine it gives the correct secret. If one is fake, it normally gives the wrong secret, with probability $1-1/p$ conditional on a uniform fake ordinate, but the inconsistency is undetectable from those $r$ shares. The data do not certify which case has occurred.

With $r+1$ shares, genuine shares are consistent with one such [polynomial](../../../../../polynomial-split.md). A fake is inconsistent with probability $1-1/p$, so it is usually detected as an inconsistency. However, omitting each of the $r+1$ shares in turn gives $r+1$ possible [polynomials](../../../../../polynomial-split.md). If the data are inconsistent, their constant terms are distinct: two candidate polynomials with the same constant term agree at zero and at their $r-1$ common abscissae, hence agree identically, which would make all the data consistent. **The secret is narrowed to $r+1$ possibilities, but the fake is not identified.**

With $r+2$ shares, at least $r+1$ are genuine. There is a unique degree-at-most-$r-1$ [polynomial](../../../../../polynomial-split.md) agreeing with at least $r+1$ shares: two candidates would agree on at least $r$ abscissae and hence coincide. Find it by deleting each share and checking consistency. **The secret is recovered uniquely, and the fake is identified unless it happens to lie on the genuine polynomial, in which case it is harmless.**

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2010](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
