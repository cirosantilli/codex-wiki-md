<h1 id="5/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Assume $0\le k\le n$ with $n,k$ integers, as required for the quantum binomial expression. Let $L_{n-1}$ be the $n$-dimensional irreducible [sl2 Lie algebra](../../../../../../sl2-lie-algebra.md) representation, with one-dimensional [weight spaces](../../../../../../weight-space.md) of [weights](../../../../../../weight-representation-theory.md) $n-1-2j$, $0\le j<n$. The [exterior-power Lie algebra representation](../../../../../../exterior-power-lie-algebra-representation.md) on $\Lambda^kL_{n-1}$ has character

$$
C_{n,k}(q)=\sum_{0\le j_1<\cdots<j_k<n}
q^{k(n-1)-2(j_1+\cdots+j_k)}.
$$

This is already a [Laurent polynomial](../../../../../../laurent-polynomial.md) with nonnegative integer coefficients.

To identify it with the requested quotient, introduce $t=q^{-2}$ and the [Gaussian binomial coefficient](../../../../../../gaussian-binomial-coefficient.md)

$$
G_{n,k}(t)=\sum_{0\le j_1<\cdots<j_k<n}
 t^{j_1+\cdots+j_k-k(k-1)/2}.
$$

Splitting the subsets according to whether $n-1$ is included proves

$$
G_{n,k}=G_{n-1,k}+t^{n-k}G_{n-1,k-1},\qquad
G_{n,0}=G_{n,n}=1.
$$

The product $\prod_{j=1}^k(1-t^{n-k+j})/(1-t^j)$ satisfies the same recurrence: after factoring common numerator and denominator terms, the needed identity is $(1-t^{n-k})+t^{n-k}(1-t^k)=1-t^n$. Induction on $n$ therefore proves the product identity, including its polynomiality.

Since the [quantum integer](../../../../../../quantum-integer.md) is $[a]_q=q^{a-1}(1-q^{-2a})/(1-q^{-2})$, taking the quotient of the products gives

$$
\boxed{\left[\begin{matrix}n\\k\end{matrix}\right]_q
=q^{k(n-k)}G_{n,k}(q^{-2})
=C_{n,k}(q)=\chi_{\Lambda^kL_{n-1}}(q).}
$$

Thus this is the [symmetric quantum binomial coefficient](../../../../../../symmetric-quantum-binomial-coefficient.md). All its [weights](../../../../../../weight-representation-theory.md) have parity $k(n-k)$, because the exponent in the exterior-power sum differs from $k(n-k)$ by an even integer. Applying part i to this finite-dimensional representation proves **symmetric unimodality in steps of two**. Equivalently, the ordinary [polynomial](../../../../../../polynomial-split.md) $G_{n,k}(t)$ has a unimodal coefficient sequence at consecutive powers of $t$.

Again, the full integer-exponent coefficient sequence in $q$, including the absent parity, need not be unimodal: for $n=2,k=1$ the answer is $q+q^{-1}$. This counterexample makes precise the convention under which the claimed quantum unimodality holds. The cases $k=0$ or $k=n$ give the constant one.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [5](../../5.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
