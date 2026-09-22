# sl2 matrix commutator example

↑ **Parent:** [Commutator](commutator.md)

Over a [field](field.md) $k$, the trace-zero $2\times2$ [matrices](matrix.md) form the [special linear Lie algebra](special-linear-lie-algebra.md) $\mathfrak{sl}_2(k)$. The [matrix trace](matrix-trace.md) of a [commutator](commutator.md) is zero, so this is a [Lie subalgebra](lie-subalgebra.md) of the [general linear Lie algebra](general-linear-lie-algebra.md). A [basis](basis.md) is

$$
H=\begin{pmatrix}1&0\\0&-1\end{pmatrix},\qquad E=\begin{pmatrix}0&1\\0&0\end{pmatrix},\qquad F=\begin{pmatrix}0&0\\1&0\end{pmatrix}.
$$

In fact $\begin{pmatrix}a&b\\c&-a\end{pmatrix}=aH+bE+cF$, uniquely. The individual products are

$$
HE=E,\quad EH=-E,\quad HF=-F,\quad FH=F,\quad EF=\begin{pmatrix}1&0\\0&0\end{pmatrix},\quad FE=\begin{pmatrix}0&0\\0&1\end{pmatrix}.
$$

Subtracting in the stated order gives

$$
[H,E]=2E,\qquad [H,F]=-2F,\qquad [E,F]=H.
$$

For [characteristic](characteristic-of-a-field.md) different from two, this is the standard [sl2 triple](sl2-triple.md); see [Etingof, Section 11.4](https://ocw.mit.edu/courses/18-755-lie-groups-and-lie-algebras-ii-spring-2024/mit18_755_s24_lec_full.pdf#page=66). The products remain valid in [characteristic two](characteristic-two.md), but there $H=I$ is central and $2E=2F=0$, so the familiar [characteristic zero](characteristic-zero.md) structure changes.

The following table gives all nine [basis](basis.md) brackets. Each entry is $[\text{row},\text{column}]$; the diagonal vanishes by alternation, and exchanging row and column reverses the sign.

| $[\ ,\ ]$ | $H$ | $E$ | $F$ |
| --- | --- | --- | --- |
| $H$ | $0$ | $2E$ | $-2F$ |
| $E$ | $-2E$ | $0$ | $H$ |
| $F$ | $2F$ | $-H$ | $0$ |

Bilinearity now computes any [commutator](commutator.md), for example

$$
[H+E,2F-E]=2[H,F]-[H,E]+2[E,F]=2H-2E-4F.
$$

The three [structure constants of a Lie algebra](structure-constant-of-a-lie-algebra.md) relations encode all of this multiplication. They also show why the [sl2 triple](sl2-triple.md) is useful in [Lie algebra representations](lie-algebra-representation.md): the actions of $E$ and $F$ move between [eigenvalues](eigenvalue.md) of the action of $H$ in steps of two.

## ↑ Ancestors (9)

1. [Commutator](commutator.md)
2. [Lie bracket](lie-bracket.md)
3. [Lie algebra](lie-algebra-split.md)
4. [Lie theory](lie-theory-split.md)
5. [Diagonal dominance](diagonal-dominance.md)
6. [Algebra](algebra-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Jacobi identity](jacobi-identity.md)
- [Lie algebra](lie-algebra-split.md)
- [Lie bracket](lie-bracket.md)
