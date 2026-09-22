<h1 id="19f/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Each $H$-conjugacy class represented by $x_i$ has $|H|/|C_H(x_i)|$ elements. For every element of that class, the number of conjugators from $g$ to it is $|C_G(g)|$. Grouping the [induced character](../../../../../../induced-character.md) formula by these classes therefore gives

$$
\boxed{(\operatorname{Ind}_H^G\psi)(g)=|C_G(g)|\sum_i\frac{\psi(x_i)}{|C_H(x_i)|}}.
$$

In the example, $a$ has order four, $b$ has order two, and $bab=a^{-1}$, so $H\cong D_8$. Its five [conjugacy classes](../../../../../../conjugacy-class.md) are $1$, $a^2$, $\{a,a^3\}$, $\{b,a^2b\}$ and $\{ab,a^3b\}$, of sizes $1,1,2,2,2$. The four one-dimensional [irreducible characters](../../../../../../irreducible-character.md) are determined by $\psi(a)=\varepsilon$ and $\psi(b)=\eta$, each sign independently chosen. The remaining two-dimensional [irreducible character](../../../../../../irreducible-character.md) comes from the plane action of the square:

$$
\begin{array}{c|rrrrr}
 &1&a^2&a&b&ab\\\hline
\psi_{\varepsilon,\eta}&1&1&\varepsilon&\eta&\varepsilon\eta\\
\psi_2&2&-2&0&0&0
\end{array}
$$

Their squared degrees sum to eight, so this is the full [character table](../../../../../../character-table.md).

In $S_4$, use class representatives $1,(12),(12)(34),(123),(1234)$. Their intersections with $H$ are respectively $\{1\}$, $\{b,a^2b\}$, $\{a^2\}\cup\{ab,a^3b\}$, the empty set, and $\{a,a^3\}$. The corresponding $S_4$ centralizer orders are $24,4,8,3,4$, while the noncentral $H$ centralizers have order four. The induced values are consequently

$$
\operatorname{Ind}\psi=(3\psi(1),\ \psi(b),\ \psi(a^2)+2\psi(ab),\ 0,\ \psi(a)).
$$

In the same $S_4$ class order, all five induced [irreducible characters](../../../../../../irreducible-character.md) are

$$
\boxed{\begin{array}{c|rrrrr}
\operatorname{Ind}\psi_{+,+}&3&1&3&0&1\\
\operatorname{Ind}\psi_{+,-}&3&-1&-1&0&1\\
\operatorname{Ind}\psi_{-,+}&3&1&-1&0&-1\\
\operatorname{Ind}\psi_{-,-}&3&-1&3&0&-1\\
\operatorname{Ind}\psi_2&6&0&-2&0&0
\end{array}}
$$

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [19F](../../19f.md)
3. [Paper 2](../../../paper-2-split.md)
4. [Ii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
