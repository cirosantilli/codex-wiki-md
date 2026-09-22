<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Tarski-Vaught test](../../../../../../tarski-vaught-test.md) states that a substructure $M\subseteq N$ is an [elementary substructure](../../../../../../elementary-substructure.md) if and only if every formula $\varphi(x,\bar y)$ and tuple $\bar a\in M$ satisfy

$$
N\models\exists x\,\varphi(x,\bar a)
\quad\Longrightarrow\quad
N\models\varphi(b,\bar a)\text{ for some }b\in M.
$$

Necessity follows immediately from elementarity. Conversely, assume the witness condition. Induct on formulas to prove that $M\models\psi(\bar a)$ exactly when $N\models\psi(\bar a)$ for every $\bar a\in M$. Atomic formulas agree because $M$ is a substructure, and Boolean connectives follow by induction. A witness in $M$ is also one in $N$; a witness in $N$ can be replaced by one in $M$ by hypothesis, after which induction applies to the matrix. Universal formulas follow by negation. Thus **the witness condition is equivalent to $M\preccurlyeq N$**.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 144](../../../paper-144-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
