<h1 id="6/solution">Solution</h1>

↑ **Parent:** [6](../6.md)

For a [unital](../../../../../unital-algebra.md) [star-subalgebra](../../../../../star-subalgebra.md) $A\subseteq B(H)$, the [Von Neumann double commutant theorem](../../../../../von-neumann-double-commutant-theorem.md) states

$$
\boxed{\overline A^{\mathrm{SOT}}=\overline A^{\mathrm{WOT}}=A''.}
$$

Here $A'$ is the [commutant of an operator algebra](../../../../../commutant-of-an-operator-algebra.md), consisting of operators commuting with every element of $A$. The double commutant is closed in either topology: multiplication by a fixed [bounded operator](../../../../../continuous-linear-operator.md) is continuous in both. Therefore both closures of $A$ lie in $A''$.

For the converse, let $T\in A''$ and choose finitely many [vectors](../../../../../vector.md) $\xi_1,\ldots,\xi_n$. In $H^n$ put

$$
K=\overline{\{(a\xi_1,\ldots,a\xi_n):a\in A\}}.
$$

It is invariant under the diagonal action of $A$ and its adjoints, so its [orthogonal projection](../../../../../orthogonal-projection.md) $Q$ commutes with that diagonal action. Consequently each [matrix](../../../../../matrix.md) entry $Q_{ij}$ belongs to $A'$. The diagonal operator with entry $T$ therefore commutes with $Q$. Since $I\in A$, the tuple $\xi=(\xi_1,\ldots,\xi_n)$ belongs to $K$, and hence so does $(T\xi_1,\ldots,T\xi_n)$. By the definition of $K$, one element $a\in A$ approximates this entire tuple arbitrarily closely. This is exactly approximation in every strong-operator neighborhood of $T$. It proves $A''\subseteq\overline A^{\mathrm{SOT}}$ and thus both asserted equalities. In particular, $M=A''$ is a [Von Neumann algebra](../../../../../von-neumann-algebra.md).

The [Kaplansky density theorem](../../../../../kaplansky-density-theorem.md) strengthens the result by preserving [norm](../../../../../norm.md) bounds:

$$
\boxed{\overline{\{a\in A:\|a\|\leq1\}}^{\mathrm{SOT}}
=\{x\in M:\|x\|\leq1\}.}
$$

It also holds for the [self-adjoint](../../../../../self-adjoint-operator.md) and positive unit balls; the full ball can in fact be approximated in the [strong-star topology](../../../../../strong-star-operator-topology.md), meaning strong convergence of both operators and adjoints. We prove the bound rather than merely scaling the unbounded approximants furnished by the double commutant theorem.

First put $C=\overline A^{\|\cdot\|}$, a [unital](../../../../../unital-algebra.md) [C-star algebra](../../../../../c-star-algebra.md). Its [self-adjoint](../../../../../self-adjoint-operator.md) part is weak-operator dense in $M_{\mathrm{sa}}$: symmetrize any weak approximating net. For a convex subset, strong and weak operator closures agree. To see this explicitly, separation from a strong [closure](../../../../../closure-topology.md) supplies a continuous real functional on finitely many image [vectors](../../../../../vector.md), hence one of the form $\operatorname{Re}\sum_j\langle a\xi_j,\eta_j\rangle$, which is also weak-operator continuous. The [Hahn-Banach separation theorem](../../../../../hahn-banach-separation-theorem.md) would then separate the point from the weak [closure](../../../../../closure-topology.md) as well. Thus every [self-adjoint](../../../../../self-adjoint-operator.md) $x\in M$ is a strong limit of [self-adjoint](../../../../../self-adjoint-operator.md) $a_i\in C$, initially without a common [norm](../../../../../norm.md) bound.

The needed functional-calculus [continuity](../../../../../continuous-function.md) follows directly from [resolvents](../../../../../resolvent-of-an-operator.md). The [resolvent identity](../../../../../resolvent-identity.md) gives

$$
(a_i-iI)^{-1}-(x-iI)^{-1}
=(a_i-iI)^{-1}(x-a_i)(x-iI)^{-1}.
$$

The first factor has [norm](../../../../../norm.md) at most one, so the right side tends strongly to zero. The same holds at $-i$. Both [resolvent](../../../../../resolvent-of-an-operator.md) nets are uniformly bounded, so their products converge strongly. Their scalar functions generate a [self-adjoint](../../../../../self-adjoint-operator.md) algebra separating points of $\mathbb R$ and vanishing at infinity. The [Stone-Weierstrass theorem](../../../../../stone-weierstrass-theorem.md), applied to the one-point compactification, makes this algebra uniformly dense in $C_0(\mathbb R)$. Uniform approximation and the functional-calculus [norm](../../../../../norm.md) bound therefore show

$$
f(a_i)\longrightarrow f(x)\text{ strongly for every }f\in C_0(\mathbb R).
$$

This proves [strong continuity of functional calculus through resolvents](../../../../../strong-continuity-of-functional-calculus-through-resolvents.md) without an unjustified uniform bound on the original $a_i$.

If $x=x^*$ and $\|x\|\leq1$, choose a real compactly supported continuous $f$ equal to the identity on $[-1,1]$ and bounded in absolute value by one. Then $f(a_i)\in C$ are [self-adjoint](../../../../../self-adjoint-operator.md) contractions and converge strongly to $f(x)=x$. For a positive contraction $x$, choose instead $0\leq f\leq1$ equal to the identity on $[0,1]$; this gives positive contractions. These prove the two restricted versions for $C$.

For an arbitrary contraction $x\in M$, apply the [self-adjoint](../../../../../self-adjoint-operator.md) result in the [matrix algebra](../../../../../matrix-algebra.md) $M_2(C)$ to

$$
X=\begin{pmatrix}0&x\\x^*&0\end{pmatrix},\qquad \|X\|=\|x\|\leq1.
$$

The strong [closure](../../../../../closure-topology.md) of $M_2(C)$ is $M_2(M)$, since finitely many entries may be approximated simultaneously. The upper-right entries $c_i$ of the approximating [self-adjoint](../../../../../self-adjoint-operator.md) contraction [matrices](../../../../../matrix.md) belong to $C$, satisfy $\|c_i\|\leq1$, and converge strongly to $x$. The lower-left entries are $c_i^*$ and converge strongly to $x^*$. This proves the full strong-star assertion for $C$.

Finally transfer the bounds from $C$ to the possibly nonclosed algebra $A$. A contraction $c\in C$ has an approximant $b\in A$ with $\|b-c\|<\varepsilon$, so $b/(1+\varepsilon)$ is an $A$-contraction within $2\varepsilon$ of $c$. [Self-adjoint](../../../../../self-adjoint-operator.md) approximants are obtained by symmetrizing first. For a positive contraction, approximate $c^{1/2}$ by $b\in A$ and use the positive contraction $b^*b/(1+\varepsilon)^2$, which tends in [norm](../../../../../norm.md) to $c$ as $\varepsilon\downarrow0$. Combining these [norm](../../../../../norm.md) approximations with each finite-vector strong approximation proves all versions for $A$. The reverse inclusions follow because the relevant [norm](../../../../../norm.md) bounds and the inequalities defining a [positive operator](../../../../../positive-operator.md) are preserved by strong limits.

## ↑ Ancestors (10)

1. [6](../6.md)
2. [Paper 1](../../paper-1-split.md)
3. [Iii](../../split.md)
4. [2008](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
