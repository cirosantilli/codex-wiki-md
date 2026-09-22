# Lambda definition of primitive recursion by pair iteration

↑ **Parent:** [Lambda definition of primitive recursion](lambda-definition-of-primitive-recursion.md)

If total [functions](function-split.md) $g$ and $h$ are represented by [lambda terms](lambda-term.md) $G,H$, define

$$
\mathsf{Step}_{\mathbf x}=\lambda p.\mathsf{Pair}(\mathsf{Succ}(\mathsf{Fst}\,p))(H\mathbf x(\mathsf{Fst}\,p)(\mathsf{Snd}\,p)),
$$

and

$$
R=\lambda\mathbf x n.\mathsf{Snd}\bigl(n\mathsf{Step}_{\mathbf x}(\mathsf{Pair}\,c_0\,(G\mathbf x))\bigr).
$$

After $j$ iterations the [Church pair](church-pair.md) holds $(c_j,c_{f(\mathbf x,j)})$, proved by [mathematical induction](mathematical-induction.md) using the defining recursion equations. Consequently $R$ represents the total [primitive recursive function](primitive-recursive-function.md) $f$. This statement concerns total inputs and total recursion constituents; it is not an unguarded composition theorem for arbitrary partial [functions](function-split.md).

## ↑ Ancestors (10)

1. [Lambda definition of primitive recursion](lambda-definition-of-primitive-recursion.md)
2. [Lambda-definable function](lambda-definable-function.md)
3. [Church numeral](church-numeral.md)
4. [Church encoding](church-encoding.md)
5. [Lambda calculus](lambda-calculus.md)
6. [Computability theory](computability-theory.md)
7. [Foundations of mathematics](foundations-of-mathematics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (5)

- [Lambda representation of partial computable functions](lambda-representation-of-partial-computable-functions.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-76/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-20/4/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-120/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-135/6/solution.md)
