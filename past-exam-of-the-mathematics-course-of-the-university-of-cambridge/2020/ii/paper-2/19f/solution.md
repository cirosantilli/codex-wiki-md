<h1 id="19f/solution">Solution</h1>

↑ **Parent:** [19F](../19f.md)

Write the [nonabelian group of order 21](../../../../../nonabelian-group-of-order-21.md) as

$$
G=\langle r,s\mid r^7=s^3=1,\ srs^{-1}=r^2\rangle
\cong C_7\rtimes C_3;
$$

replacing $2$ by $4$ gives the same group. Conjugation by $s$ splits the six nonidentity elements of the normal subgroup $\langle r\rangle$ into the two classes

$$
C_1=\{r,r^2,r^4\},\qquad
C_2=\{r^3,r^5,r^6\}.
$$

Each of the two other cosets is one conjugacy class:

$$
C_3=\langle r\rangle s,\qquad C_4=\langle r\rangle s^2.
$$

Thus the class sizes are $1,3,3,7,7$, so there are five [irreducible characters](../../../../../irreducible-representation.md).

The [abelianization](../../../../../abelianization.md) is $C_3$, giving three [linear characters](../../../../../linear-character.md). Put $\omega=e^{2\pi i/3}$ and $\zeta=e^{2\pi i/7}$, and define

$$
\alpha=\zeta+\zeta^2+\zeta^4=\frac{-1+i\sqrt7}{2},
\qquad
\beta=\zeta^3+\zeta^5+\zeta^6=\frac{-1-i\sqrt7}{2}.
$$

The two nontrivial orbits of characters of the normal $C_7$ induce two irreducible characters of degree three. Their values vanish outside $C_7$, and summing each orbit gives $\alpha,\beta$ on the two nonidentity classes. The resulting [character table](../../../../../character-table.md) is

$$
\begin{array}{c|ccccc}
&1&C_1&C_2&C_3&C_4\\
\hline
|C|&1&3&3&7&7\\
\chi_1&1&1&1&1&1\\
\chi_2&1&1&1&\omega&\omega^2\\
\chi_3&1&1&1&\omega^2&\omega\\
\chi_4&3&\alpha&\beta&0&0\\
\chi_5&3&\beta&\alpha&0&0
\end{array}.
$$

The degree check

$$
1^2+1^2+1^2+3^2+3^2=21
$$

and [character orthogonality relations](../../../../../character-orthogonality.md) verify that this is the complete table.

## ↑ Ancestors (10)

1. [19F](../19f.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ii](../../split.md)
4. [2020](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
