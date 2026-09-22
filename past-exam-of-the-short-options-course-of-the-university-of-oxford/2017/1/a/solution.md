<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For distinct [odd primes](../../../../odd-prime.md) $p,q$, [quadratic reciprocity](../../../../quadratic-reciprocity.md) states

$$
\boxed{\left(\frac pq\right)\left(\frac qp\right)=(-1)^{(p-1)(q-1)/4}.}
$$

Here the [Legendre symbol](../../../../legendre-symbol.md) records whether a nonzero [congruence class](../../../../congruence-class.md) is a [quadratic residue](../../../../quadratic-residue-split.md). The [first supplementary law for quadratic reciprocity](../../../../first-supplementary-law-for-quadratic-reciprocity.md) and [second supplementary law for quadratic reciprocity](../../../../second-supplementary-law-for-quadratic-reciprocity.md) give

$$
\left(\frac{-1}p\right)=(-1)^{(p-1)/2},\qquad
\left(\frac2p\right)=(-1)^{(p^2-1)/8}.
$$

Thus **minus one is a square exactly when $p\equiv1\pmod4$, and two is a square exactly when $p\equiv1$ or $7\pmod8$**.

To test the specified [congruence class](../../../../congruence-class.md), factor $111=3\cdot37$. Since $2017\equiv1\pmod4$, [multiplicativity of the Legendre symbol](../../../../multiplicativity-of-the-legendre-symbol.md) and [quadratic reciprocity](../../../../quadratic-reciprocity.md) yield

$$
\begin{aligned}
\left(\frac{111}{2017}\right)
&=\left(\frac3{2017}\right)\left(\frac{37}{2017}\right)
=\left(\frac{2017}3\right)\left(\frac{2017}{37}\right)\\
&=\left(\frac13\right)\left(\frac{19}{37}\right)
=\left(\frac{37}{19}\right)
=\left(\frac{18}{19}\right).
\end{aligned}
$$

There is no sign change on swapping $19$ and $37$ because $37\equiv1\pmod4$. Finally $18=2\cdot3^2$, so [multiplicativity of the Legendre symbol](../../../../multiplicativity-of-the-legendre-symbol.md) gives $(18/19)=(2/19)=-1$, since $19\equiv3\pmod8$. Therefore

$$
\boxed{x^2\equiv111\pmod{2017}\text{ has no integer solution}.}
$$

## ↑ Ancestors (12)

1. [A](../a.md)
2. [1](../../1.md)
3. [2017](../../../2017-split.md)
4. [Past exam of the short options course of the University of Oxford](../../../split.md)
5. [Short options course of the University of Oxford](../../../../short-options-course-of-the-university-of-oxford.md)
6. [Year 2 of the mathematics course of the University of Oxford](../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
