<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Roth theorem](../../../../../../roth-s-theorem.md) states that if $\alpha$ is a real algebraic irrational number, then for every $\varepsilon>0$ there are only finitely many reduced fractions $p/q$ satisfying

$$
\left|\alpha-\frac pq\right|<q^{-2-\varepsilon}.
$$

To derive this from the [Schmidt subspace theorem](../../../../../../schmidt-subspace-theorem.md), take

$$
L_1(X,Y)=X-\alpha Y,
\qquad
L_2(X,Y)=Y.
$$

These forms are linearly independent. For a solution $(p,q)$ with $q$ large, $|p|\asymp q$, so $H(p,q)\asymp q$, while

$$
|L_1(p,q)L_2(p,q)|
=|p-\alpha q|q
=q^2\left|\alpha-\frac pq\right|
<q^{-\varepsilon}.
$$

After slightly decreasing $\varepsilon$, the [Schmidt subspace theorem](../../../../../../schmidt-subspace-theorem.md) puts all such primitive vectors $(p,q)$ in finitely many rational lines. Each rational line contains only the two opposite primitive integer vectors $\pm(p,q)$, and these determine the same fraction. Hence only finitely many fractions occur.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 166](../../../paper-166-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
