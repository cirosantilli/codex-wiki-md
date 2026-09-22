<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The structural induction principle says that a property $P(f)$ holds for every [primitive recursive function](../../../../../../primitive-recursive-function.md) if it holds for every [initial function of recursion theory](../../../../../../initial-function-of-recursion-theory.md) and is preserved by [function composition in recursion theory](../../../../../../function-composition-in-recursion-theory.md) and [primitive recursion](../../../../../../primitive-recursion.md). This is justified because primitive recursive functions are, by definition, the smallest class closed under those constructors; equivalently, every such function has a finite construction tree, and ordinary induction on its height proves $P$.

Take $P(f)$ to mean that $f$ is total. The zero, successor, and projection functions are total. A composition of total functions is total. Finally, suppose $g$ and $h$ are total and $f$ is defined from them by primitive recursion. For fixed $\mathbf x$, induction on $n$ proves that $f(\mathbf x,n)$ exists: the value at zero is $g(\mathbf x)$, and from the existing value at $n$, totality of $h$ gives the value at $n+1$. Therefore [every primitive recursive function is total](../../../../../../every-primitive-recursive-function-is-total.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 120](../../../paper-120-split.md)
4. [Iii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
