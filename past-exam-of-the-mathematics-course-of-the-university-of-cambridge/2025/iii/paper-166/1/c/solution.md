<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let

$$
\phi=\frac{1+\sqrt5}{2},
\qquad
\psi=\frac{1-\sqrt5}{2}=-\phi^{-1}.
$$

Suppose $F_n=x^k$ is a [perfect power](../../../../../../perfect-power.md) with $x\geq2$. The finitely many small $n$ can be absorbed into the final effective constant. The [Binet formula](../../../../../../binet-formula.md) gives $x^k\asymp\phi^n$ and

$$
\left|\frac{\phi^n}{\sqrt5x^k}-1\right|
=\frac{|\psi|^n}{\sqrt5x^k}
\ll\phi^{-2n}.
$$

Thus, for

$$
\Lambda=n\log\phi-\log\sqrt5-k\log x,
$$

the local Lipschitz equivalence of $u$ and $e^u-1$ at zero yields

$$
0<|\Lambda|\ll\phi^{-2n}.
$$

The form cannot vanish: applying the nontrivial [field automorphism](../../../../../../field-automorphism.md) of $\mathbb Q(\sqrt5)$ to $\phi^n=\sqrt5x^k$ would give $\psi^n=-\sqrt5x^k$, whose absolute values are incompatible.

Apply the [Baker lower bound for a homogeneous linear form in logarithms](../../../../../../baker-lower-bound-for-a-homogeneous-linear-form-in-logarithms.md) with the variable-height number $x$ placed last. The parameters belonging to $\phi$ and $\sqrt5$ are absolute constants, while $\log A_x\asymp\log x$. Moreover,

$$
k\log x=n\log\phi+O(1),
$$

so $n/\log A_x\ll k$ and therefore $B^*\ll k$. The refined lower bound becomes

$$
|\Lambda|>\exp(-C_1\log x\log k)
>\exp\!\left(-C_2\frac nk\log k\right).
$$

Comparison with the exponential upper bound gives $k\leq C_3\log k$. Since $k/\log k$ tends to infinity, this bounds $k$ by an effective absolute constant. Enlarging it to cover the discarded small indices proves the claim.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
