<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Let $V$ afford the given [group representation](../../../../../../group-representation.md) of $H$. Its [induced representation](../../../../../../induced-representation.md) is the left $G$-module

$$
\boxed{\operatorname{Ind}_H^G V=\mathbb C[G]\otimes_{\mathbb C[H]}V}.
$$

Choose representatives $t$ of the left cosets $G/H$; then it is the direct sum of the spaces $t\otimes V$. If $gt=t'h$ with $h\in H$, the action sends $t\otimes v$ to $t'\otimes\Psi(h)v$. This is independent of the representatives up to equivalence, and its dimension is $[G:H]\dim V$.

Only cosets fixed by $g$ contribute to its trace. Their contribution is $\psi(t^{-1}gt)$, giving the [induced character](../../../../../../induced-character.md) formula

$$
\boxed{\psi^G(g)=\sum_{\substack{tH\in G/H\\t^{-1}gt\in H}}\psi(t^{-1}gt)
=\frac1{|H|}\sum_{\substack{x\in G\\x^{-1}gx\in H}}\psi(x^{-1}gx)}.
$$

For an arbitrary [class function](../../../../../../class-function.md) $f$ on $H$, the same averaging formula defines its induced [class function](../../../../../../class-function.md) on $G$. Equivalently, extend $f$ by zero outside $H$ and average $|H|^{-1}\sum_x f(x^{-1}gx)$. This definition is linear and does not require $f$ to be an actual [character](../../../../../../character-of-a-representation.md).

For a complex [character](../../../../../../character-of-a-representation.md) $\psi$ of a [finite group](../../../../../../finite-group.md) $G$ afforded by a [representation](../../../../../../group-representation.md) $\rho$, its [determinant character](../../../../../../determinant-character.md) is

$$
\boxed{(\det\psi)(g)=\det\rho(g)}.
$$

Multiplicativity of the determinant makes this a [linear character](../../../../../../linear-character.md); it does not mean the determinant of the scalar value $\psi(g)$. The definition depends only on the [character](../../../../../../character-of-a-representation.md) because [characters](../../../../../../character-of-a-representation.md) determine the equivalence class of a finite-dimensional complex [representation](../../../../../../group-representation.md). In particular the [determinant character](../../../../../../determinant-character.md) is trivial on the [derived subgroup](../../../../../../commutator-subgroup.md) $G'$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
