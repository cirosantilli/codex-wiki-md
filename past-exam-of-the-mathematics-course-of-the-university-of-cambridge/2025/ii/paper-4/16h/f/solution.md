<h1 id="16h/f/solution">Solution</h1>

↑ **Parent:** [F](../f.md)

Take

$$
\varphi^*=\varphi^M,
$$

the [formula relativization to a class](../../../../../../formula-relativization-to-a-class.md): replace each $\exists y\,\psi$ by

$$
\exists y\,(y\in M\land\psi^M)
$$

and each $\forall y\,\psi$ by

$$
\forall y\,(y\in M\mathbin\Rightarrow\psi^M),
$$

leaving atomic formulas unchanged. If $M$ is given by a defining formula, insert that formula wherever $y\in M$ occurs; this is why the map may depend on $M$.

For $z$ and any parameters in $M$, induction on formulas gives

$$
V\models\varphi^M(z)
\quad\Longleftrightarrow\quad
M\models\varphi(z).
$$

Therefore $\varphi^*$-closure puts

$$
\{z\in x:V\models\varphi^M(z)\}
=\{z\in x:M\models\varphi(z)\}
$$

in $M$ for every $x\in M$. This is exactly the [relativized closure criterion for separation](../../../../../../relativized-closure-criterion-for-separation.md), so $(M,\in)$ satisfies the $\varphi$-instance of separation.

## ↑ Ancestors (11)

1. [F](../f.md)
2. [16H](../../16h.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
