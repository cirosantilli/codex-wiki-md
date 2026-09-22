<h1 id="2/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $p=2$, the even residue class contains exactly one root, by the simple-root form of [Hensel lemma](../../../../../../hensel-s-lemma.md) at $a=0$: $f(0)=20$ and $f'(0)=-5$ is a unit. For the odd classes use the [strong form of Hensel lemma](../../../../../../strong-form-of-hensel-lemma.md):

$$
f(1)=16,\quad f'(1)=-2;\qquad f(3)=32,\quad f'(3)=22.
$$

In both cases $v_2(f(a))>2v_2(f'(a))=2$. Each gives exactly one root in $a+4\mathbb Z_2$. These two balls partition the odd integers, so there are no further roots.

For $p=3$, reduction gives $\overline f=X^3+X+2$, whose sole root is $2$. The derivative $3X^2-5$ is always a unit modulo $3$, so that root lifts uniquely. For $p=5$, the only possible residue is zero. But if $x\in5\mathbb Z_5$, then $x^3-5x\in25\mathbb Z_5$ while $20$ has valuation one, so $f(x)$ cannot vanish. **The exact root counts are**

$$
\boxed{\#\{f=0\text{ in }\mathbb Z_2\}=3,\quad \#\{f=0\text{ in }\mathbb Z_3\}=1,\quad \#\{f=0\text{ in }\mathbb Z_5\}=0.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [2](../../2.md)
3. [Paper 28](../../../paper-28-split.md)
4. [Iii](../../../split.md)
5. [2012](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
