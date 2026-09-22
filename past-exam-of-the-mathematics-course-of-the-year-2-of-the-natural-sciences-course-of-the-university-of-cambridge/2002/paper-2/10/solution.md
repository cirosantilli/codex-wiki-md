<h1 id="10/solution">Solution</h1>

↑ **Parent:** [10](../10.md)

**Definitions and labels.** A complex [group representation](../../../../group-representation.md) on a vector space $V$ is a [group homomorphism](../../../../group-homomorphism.md) $\rho:G\to\operatorname{GL}(V)$, so $\rho(gh)=\rho(g)\rho(h)$ and $\rho(e)=I$. It is an [irreducible representation](../../../../irreducible-representation.md) if $V\ne0$ and its only invariant subspaces are $0$ and $V$.

Read permutation matrices by their action on column basis vectors. The labels in the original PDF are

$$
I=e,\quad A=(123),\quad B=(132),\quad C=(13),\quad D=(12),\quad E=(23).
$$

In particular, the original PDF gives the last row of $C$ as $(1,0,0)$; the provided TeX transcription's $(0,0,1)$ is incorrect and would not give an invertible permutation matrix.

**Multiplication and conjugacy.** Matrix products act on columns with the right factor first. For example $A^2=B$, $AD=C$, and $DA=E$. The complete [multiplication table](../../../../multiplication-table.md), with row factor multiplied by column factor, is

$$
\boxed{\begin{array}{c|rrrrrr}
 &I&A&B&C&D&E\\\hline
I&I&A&B&C&D&E\\
A&A&B&I&E&C&D\\
B&B&I&A&D&E&C\\
C&C&D&E&I&A&B\\
D&D&E&C&B&I&A\\
E&E&C&D&A&B&I
\end{array}.}
$$

Conjugating a [permutation](../../../../permutation.md) relabels its cycles. Thus the [conjugacy classes](../../../../conjugacy-class.md) are

$$
\boxed{\{I\},\qquad\{A,B\},\qquad\{C,D,E\},}
$$

of sizes one, two and three. These are respectively the identity, the three-cycles and the transpositions in the [symmetric group on three letters](../../../../symmetric-group-on-three-points.md).

**Dimensions.** The [sum of squares of irreducible representation dimensions](../../../../sum-of-squares-of-irreducible-representation-dimensions.md) equals the [group order](../../../../order-of-a-finite-group.md), which here is six. A three-dimensional [irreducible representation](../../../../irreducible-representation.md) would already contribute nine, so the displayed representation is reducible. There are three inequivalent complex [irreducible representations](../../../../irreducible-representation.md), one for each [conjugacy class](../../../../conjugacy-class.md), including the [trivial representation](../../../../trivial-representation.md) of dimension one. If their dimensions are $1,d_2,d_3$, then $d_2^2+d_3^2=5$, whose positive integer solution is $\{d_2,d_3\}=\{1,2\}$. Hence

$$
\boxed{\text{irreducible dimensions: }1,1,2.}
$$

One can also see reducibility directly: every permutation matrix fixes $(1,1,1)^T$.

**Characters.** The [character of a representation](../../../../character-of-a-representation.md) is the [trace](../../../../matrix-trace.md) of its representing matrix, constant on each [conjugacy class](../../../../conjugacy-class.md). The given [permutation representation](../../../../permutation-representation.md) has character equal to the number of fixed basis vectors:

$$
\boxed{\chi_{\rm perm}=(3,0,1)}
$$

in class order $(I;A,B;C,D,E)$. A [trivial representation](../../../../trivial-representation.md) has character $(1,1,1)$. For the second one-dimensional character, a transposition has value $\pm1$ because its square is the identity. The two three-cycles are conjugate and inverse, so their common value $a$ obeys both $a^2=1$ and $a^3=1$, forcing $a=1$. [Character orthogonality](../../../../character-orthogonality.md) with the trivial character then requires $1+2+3b=0$, giving $b=-1$. This determines the [sign representation](../../../../sign-representation.md) without constructing its matrices.

Write the two-dimensional character as $(2,x,y)$. [Character orthogonality](../../../../character-orthogonality.md) with the first two rows gives

$$
2+2x+3y=0,\qquad2+2x-3y=0,
$$

so $x=-1$, $y=0$. Its squared norm is $(4+2)/6=1$, as required. The complete [character table](../../../../character-table.md) is therefore

$$
\boxed{\begin{array}{c|rrr}
\text{class}&I&A,B&C,D,E\\\hline
\text{class size}&1&2&3\\\hline
\chi_{\rm triv}&1&1&1\\
\chi_{\rm sign}&1&1&-1\\
\chi_{\rm std}&2&-1&0
\end{array}.}
$$

The last row belongs to the [standard representation of the symmetric group](../../../../standard-representation-of-the-symmetric-group.md).

To decompose the given representation, use the [character inner product](../../../../character-inner-product.md)

$$
\langle\chi,\psi\rangle=\frac16\left[\chi(I)\overline{\psi(I)}+2\chi(A)\overline{\psi(A)}+3\chi(C)\overline{\psi(C)}\right].
$$

Its multiplicities are

$$
\langle\chi_{\rm perm},\chi_{\rm triv}\rangle=\frac{3+3}{6}=1,\qquad
\langle\chi_{\rm perm},\chi_{\rm sign}\rangle=\frac{3-3}{6}=0,\qquad
\langle\chi_{\rm perm},\chi_{\rm std}\rangle=\frac6{6}=1.
$$

Thus

$$
\boxed{\rho_{\rm perm}\cong\mathbf1_{\rm triv}\oplus\rho_{\rm std},\qquad3=1+2.}
$$

Concretely the invariant line is spanned by $(1,1,1)^T$ and its invariant complement is $\{(x,y,z):x+y+z=0\}$. Their characters are exactly the first and third rows, agreeing with the decomposition obtained entirely from [character orthogonality](../../../../character-orthogonality.md).

## ↑ Ancestors (12)

1. [10](../10.md)
2. [Paper 2](../../paper-2-split.md)
3. [2002](../../split.md)
4. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../split.md)
5. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
6. [Year 2 of the natural sciences course of the University of Cambridge](../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year of the natural sciences course of the University of Cambridge](../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Natural sciences course of the University of Cambridge](../../../../natural-sciences-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
