<h1 id="5e/solution">Solution</h1>

↑ **Parent:** [5E](../5e.md)

For finite sets $A_1,\ldots,A_s$, the [inclusion-exclusion principle](../../../../../inclusion-exclusion-principle.md) states

$$
\left|\bigcup_{i=1}^sA_i\right|
=\sum_{\varnothing\ne J\subseteq\{1,\ldots,s\}}
(-1)^{|J|+1}\left|\bigcap_{j\in J}A_j\right|.
$$

To prove it, consider an element belonging to exactly $d$ of the sets. If $d=0$, it contributes zero to both sides. If $d>0$, its contribution on the right is

$$
\sum_{j=1}^d(-1)^{j+1}\binom dj=1-(1-1)^d=1,
$$

which is its contribution to the union. Summing these contributions proves the formula.

For the keypad, a first digit zero cannot be entered. Define four families of valid codes: $A$ consists of all codes with no zero; $B$ consists of codes beginning with $2$; $C$ consists of $110b$ with $b\in\{1,\ldots,9\}$; and $D$ consists of $a110$ with $a\in\{1,\ldots,9\}$. They cover every valid code. Indeed, if the first digit is not $2$, a zero in the second position is impossible; a zero in the third requires the prefix $11$; a zero in the fourth requires the middle pair $11$. In the third-position case the last digit cannot also be zero. Hence the only remaining zero-containing possibilities are exactly $C$ and $D$.

Their cardinalities are

$$
|A|=9^4=6561,\quad |B|=10^3=1000,\quad |C|=9,\quad |D|=9.
$$

The only nonempty pairwise intersections are $A\cap B$, with $9^3=729$ codes, and $B\cap D=\{2110\}$, with one code. All triple and fourfold intersections are empty. Applying [inclusion-exclusion](../../../../../inclusion-exclusion-principle.md) therefore gives

$$
\boxed{6561+1000+9+9-729-1=6849\text{ enterable codes}.}
$$

The restriction concerns actual preceding keypresses. It cannot license two successive zeros unless the first-key condition is already satisfied.

## ↑ Ancestors (10)

1. [5E](../5e.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ia](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
