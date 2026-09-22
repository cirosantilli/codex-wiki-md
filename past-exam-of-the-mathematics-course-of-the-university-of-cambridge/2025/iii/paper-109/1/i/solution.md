<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Every positive integer $m$ has a unique [binomial representation](../../../../../../combinatorial-number-system.md)

$$
m=\binom{a_r}{r}+\binom{a_{r-1}}{r-1}+\cdots+\binom{a_s}{s},
\qquad a_r>a_{r-1}>\cdots>a_s\geq s\geq1.
$$

Define

$$
f_r(m)=\binom{a_r}{r-1}+\binom{a_{r-1}}{r-2}+\cdots+\binom{a_s}{s-1}.
$$

The [Kruskal-Katona theorem](../../../../../../kruskal-katona-theorem.md) says that every $r$-uniform family $\mathcal A$ of size $m$ has

$$
|\partial\mathcal A|\geq f_r(m),
$$

and the initial segment of length $m$ in [colexicographic order](../../../../../../colexicographic-order.md) attains equality.

We prove the inequality by simultaneous [mathematical induction](../../../../../../mathematical-induction.md) on the ground-set size and on $r$. We use the elementary [binomial-shadow arithmetic lemma](../../../../../../binomial-shadow-arithmetic-lemma.md)

$$
f_r(a+b)\leq\max\{f_r(a),b\}+f_{r-1}(b).
$$

To verify the lemma, greedily remove the largest term $\binom qr$ from the binomial representation of $a+b$. If $a$ reaches that term first, apply the induction hypothesis to the remainders; otherwise transfer the excess to $b$. In the crossing case [Pascal's identity](../../../../../../pascal-s-rule.md)

$$
\binom qr=\binom{q-1}r+\binom{q-1}{r-1}
$$

gives exactly the two terms on the right. This induction also proves uniqueness of the greedy representation.

Choose the largest ground-set element $x$ and split

$$
\mathcal A_0=\{A\in\mathcal A:x\notin A\},
\qquad
\mathcal A_1=\{A\setminus\{x\}:x\in A\}.
$$

The members of the lower shadow that avoid $x$ form $\partial\mathcal A_0\cup\mathcal A_1$, while those containing $x$ are the sets $B\cup\{x\}$ with $B\in\partial\mathcal A_1$. Hence, writing $a=|\mathcal A_0|$ and $b=|\mathcal A_1|$,

$$
|\partial\mathcal A|
=|\partial\mathcal A_0\cup\mathcal A_1|+|\partial\mathcal A_1|
\geq\max\{f_r(a),b\}+f_{r-1}(b)
\geq f_r(a+b).
$$

This completes the induction.

Finally, the initial colex segment first contains all $r$-subsets of $[a_r]$, followed recursively by sets containing $a_r+1$ whose remaining elements form the appropriate initial segment at level $r-1$. Its shadow has the same recursive decomposition, and therefore has exactly $f_r(m)$ members. This proves sharpness.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [1](../../1.md)
3. [Paper 109](../../../paper-109-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
