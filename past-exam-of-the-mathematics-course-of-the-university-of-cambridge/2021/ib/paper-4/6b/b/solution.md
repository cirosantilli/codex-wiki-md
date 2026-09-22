<h1 id="6b/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Appending the node $-2$ to the existing [Newton interpolation polynomial](../../../../../../newton-polynomial.md) gives

$$
p_4(x)=p_3(x)+a_4x(x-1)(x-2)(x-3).
$$

At the new node,

$$
p_3(-2)=-82,
\qquad
(-2)(-3)(-4)(-5)=120.
$$

The condition $p_4(-2)=10$ therefore gives

$$
a_4=\frac{10-(-82)}{120}=\frac{23}{30}.
$$

Hence

$$
\boxed{
p_4(x)=4x-3x(x-1)+\frac73x(x-1)(x-2)
+\frac{23}{30}x(x-1)(x-2)(x-3)
}.
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [6B](../../6b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ib](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
