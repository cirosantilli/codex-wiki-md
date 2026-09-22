<h1 id="5/solution">Solution</h1>

↑ **Parent:** [5](../5.md)

[Ordinal arithmetic](../../../../../ordinal-arithmetic.md) describes the order types of well-ordered constructions. Its operations are defined by [transfinite recursion](../../../../../transfinite-recursion.md), continuous in their right argument at limits. For addition,

$$
\alpha+0=\alpha,\quad\alpha+(\beta+1)=(\alpha+\beta)+1,\quad\alpha+\lambda=\sup_{\beta<\lambda}(\alpha+\beta).
$$

For multiplication,

$$
\alpha\cdot0=0,\quad\alpha\cdot(\beta+1)=\alpha\cdot\beta+\alpha,\quad\alpha\cdot\lambda=\sup_{\beta<\lambda}\alpha\cdot\beta,
$$

and, for $\alpha>0$, exponentiation is defined by

$$
\alpha^0=1,\quad\alpha^{\beta+1}=\alpha^\beta\cdot\alpha,\quad\alpha^\lambda=\sup_{\beta<\lambda}\alpha^\beta.
$$

The usual conventions give $0^0=1$ and $0^\beta=0$ for $\beta>0$. [Ordinal addition](../../../../../ordinal-addition.md) concatenates orders, while [ordinal multiplication](../../../../../ordinal-multiplication.md) takes a succession of copies of the left factor indexed by the right factor.

[Ordinal addition](../../../../../ordinal-addition.md) and [ordinal multiplication](../../../../../ordinal-multiplication.md) are associative but generally not commutative; exponentiation is not an associative operation. For example,

$$
1+\omega=\omega<\omega+1,\qquad 2\cdot\omega=\omega<\omega\cdot2.
$$

The distributive identity is $\alpha(\beta+\gamma)=\alpha\beta+\alpha\gamma$; the reversed distributive law fails, since $(1+1)\omega=\omega$ but $1\omega+1\omega=\omega\cdot2$. For positive bases, $\alpha^{\beta+\gamma}=\alpha^\beta\alpha^\gamma$ follows from the recursive definitions. These are order-type identities, not an extension of commutative integer arithmetic.

Every nonzero [ordinal](../../../../../ordinal.md) has a unique [Cantor normal form](../../../../../cantor-normal-form.md)

$$
\alpha=\omega^{\alpha_1}c_1+\cdots+\omega^{\alpha_r}c_r,\qquad\alpha_1>\cdots>\alpha_r,\quad c_j\in\mathbb N_{>0}.
$$

Comparisons are lexicographic in the exponent/coefficient list. Adding a later ordinal can erase smaller final terms of the earlier one, explaining noncommutativity. [Hessenberg natural sum](../../../../../hessenberg-natural-sum.md) instead aligns equal exponents and adds their coefficients, producing a commutative operation. Finite recursive expressions formed from zero, sums and powers of $\omega$ describe exactly the [ordinals](../../../../../ordinal.md) below [epsilon zero](../../../../../epsilon-zero.md), the least positive solution of $\omega^\alpha=\alpha$. With $\omega_0=1$ and $\omega_{m+1}=\omega^{\omega_m}$,

$$
\varepsilon_0=\sup_m\omega_m.
$$

To use these ordinals computationally, fix effective [fundamental sequences of limit ordinals](../../../../../fundamental-sequence-of-a-limit-ordinal.md). Write a nonzero limit below $\varepsilon_0$ as $\gamma+\omega^\beta$, where this is its last Cantor term with one copy separated off. If $\beta=\delta+1$, set

$$
(\gamma+\omega^{\delta+1})[n]=\gamma+\omega^\delta(n+1).
$$

If $\beta$ is a nonzero limit, set $(\gamma+\omega^\beta)[n]=\gamma+\omega^{\beta[n]}$. These sequences increase to their limit; for instance $\omega[n]=n+1$ and $(\omega^\omega)[n]=\omega^{n+1}$. At the endpoint choose $\varepsilon_0[n]=\omega_{n+1}$. The shift by one is a convention; changing it changes exact finite values, so it must be specified.

The [fast-growing hierarchy](../../../../../fast-growing-hierarchy.md) now combines iteration at successors with diagonalization at limits:

$$
\boxed{F_0(n)=n+1,\qquad F_{\alpha+1}(n)=F_\alpha^{\,n+1}(n),\qquad F_\lambda(n)=F_{\lambda[n]}(n).}
$$

The superscript denotes repeated function composition, not exponentiation. Thus

$$
F_1(n)=2n+1,\qquad F_2(n)=2^{n+1}(n+1)-1.
$$

The next level iterates an exponential-growth function $n+1$ times, yielding tower-like growth; further finite levels iterate the corresponding higher growth. Each fixed finite level is [primitive recursive](../../../../../primitive-recursive-function.md), and every unary [primitive recursive function](../../../../../primitive-recursive-function.md) is eventually dominated by a sufficiently high finite level. The first limit diagonalizes over all of them: $F_\omega(n)=F_{n+1}(n)$ has Ackermannian growth and is not primitive recursive. Further limits give diagonals over already transfinite stretches of the hierarchy.

[Transfinite induction](../../../../../transfinite-induction.md) proves totality for every fixed ordinal index in the chosen well-founded notation system: limit evaluation passes to a smaller index, while successor evaluation performs finitely many calls at the preceding index. For the standard fundamental sequences, $\alpha<\beta$ implies $F_\alpha(n)<F_\beta(n)$ for all sufficiently large $n$. This [eventual dominance in a fast-growing hierarchy](../../../../../eventual-dominance-in-a-fast-growing-hierarchy.md) is not pointwise monotonicity in the ordinal index. For example,

$$
F_\omega(1)=F_2(1)=7<2047=F_3(1),
$$

even though $3<\omega$.

The hierarchy also measures proof-theoretic strength. Every fixed $F_\alpha$ with $\alpha<\varepsilon_0$ is provably total in [Peano arithmetic](../../../../../peano-arithmetic.md), and every number-theoretic function provably total there is eventually majorized by some such level. The endpoint $F_{\varepsilon_0}$ is a total recursive function in the usual mathematical metatheory but its totality is not provable in consistent PA. The classification is established in [https://epub.ub.uni-muenchen.de/3843/1/3843.pdf](https://epub.ub.uni-muenchen.de/3843/1/3843.pdf) . The distinction is between separately proving each fixed lower level and proving one uniform diagonal statement covering all lower levels; a theory cannot interchange those quantifiers without additional strength.

A related example is [Goodstein's theorem](../../../../../goodstein-s-theorem.md). Changing the base in a [hereditary base representation](../../../../../hereditary-base-representation.md) can increase the natural number dramatically, but replacing that base by $\omega$ gives an [ordinal rank of a Goodstein term](../../../../../ordinal-rank-of-a-goodstein-term.md) below $\varepsilon_0$. Subtracting one strictly decreases this rank, so an infinite nonterminating process would give an impossible ordinal descent. This illustrates the central connection: **ordinal descent proves termination while fast-growing hierarchies measure how long finite terminating processes can last**. The size of intermediate natural numbers need not resemble the simplicity of their ordinal termination measure.

## ↑ Ancestors (10)

1. [5](../5.md)
2. [Paper 18](../../paper-18-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
