<h1 id="1c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

An [integer](../../../../../../integer.md) square is divisible by four exactly when its base is even: an even base has square $4j^2$, while an odd base has square $(2j+1)^2\equiv1\pmod4$. Apply this observation to the [triangular number](../../../../../../triangular-number.md) $T_n$ obtained above. Since $n(n+1)$ is even,

$$
4\mid T_n^2\quad\Longleftrightarrow\quad 2\mid T_n\quad\Longleftrightarrow\quad4\mid n(n+1).
$$

Checking the four [residue classes](../../../../../../residue-class.md) of $n$ modulo four, the products $n(n+1)$ have residues $0,2,2,0$, respectively. Therefore

$$
\boxed{4\mid\sum_{r=1}^n r^3\quad\Longleftrightarrow\quad n\equiv0\text{ or }3\pmod4}.
$$

The original PDF has two alternatives modulo four; the TeX transcription incorrectly turns the second alternative into a modulus-three expression.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1C](../../1c.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
