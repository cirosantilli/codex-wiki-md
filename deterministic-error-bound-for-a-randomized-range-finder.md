# Deterministic error bound for a randomized range finder

↑ **Parent:** [Randomized range finder](randomized-range-finder.md)

Split a thin [singular value decomposition](singular-value-decomposition.md) at $\ell$, writing $A=U_aD_aV_a^T+U_bD_bV_b^T$ and $\Omega_i=V_i^TX$. Suppose $\Omega_a$ has [full row rank](full-row-rank.md) and the [column space](column-space.md) of $Q$ contains that of $AX$. With $P=QQ^T$, the identity $(I-P)AX=0$ and the [Moore-Penrose pseudoinverse](moore-penrose-inverse.md) give

$$
(I-P)A=(I-P)U_bD_b[-\Omega_b\Omega_a^\dagger\ \ I]V^T.
$$

Since $\|D_b\|_2=\sigma_{\ell+1}$, [submultiplicativity of the operator norm](submultiplicativity-of-the-operator-norm.md) gives the displayed bound: $[-F\ I][-F\ I]^T=FF^T+I$ proves $\|[-F\ I]\|_2=\sqrt{1+\|F\|_2^2}$. This statement is deterministic. A Gaussian error estimate needs a separate [probability](probability.md) bound on the two random factors.

## ↑ Ancestors (7)

1. [Randomized range finder](randomized-range-finder.md)
2. [Low-rank approximation](low-rank-approximation.md)
3. [Linear algebra](linear-algebra-split.md)
4. [Algebra](algebra-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-numerical-linear-algebra-course-of-the-university-of-oxford/2025/2/b/v/solution.md)
