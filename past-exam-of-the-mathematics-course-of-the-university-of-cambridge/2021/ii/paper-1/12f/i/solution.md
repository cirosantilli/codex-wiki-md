<h1 id="12f/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [partial recursive function](../../../../../../computable-function.md) is obtained from the three kinds of [initial function of recursion theory](../../../../../../initial-function-of-recursion-theory.md)—  
the [zero function](../../../../../../zero-function.md), [successor function](../../../../../../successor-function.md), and [projection function](../../../../../../projection-function.md)—by finitely many applications of [function composition in recursion theory](../../../../../../function-composition-in-recursion-theory.md), [primitive recursion](../../../../../../primitive-recursion.md), and [unbounded minimization](../../../../../../mu-operator.md). Explicitly, primitive recursion has the form

$$
f(\mathbf x,0)=g(\mathbf x),
\qquad
f(\mathbf x,n+1)=h(\mathbf x,n,f(\mathbf x,n)),
$$

while minimization takes the least $y$ for which $g(\mathbf x,y)=0$ and is undefined if no such $y$ is found.

For the function in part (i), define

$$
s(0)=1,
\qquad
s(n+1)=0.
$$

The initial value $1=S(Z(0))$ and the identically zero recursion step are [primitive recursive](../../../../../../primitive-recursive-function.md), so this is a primitive-recursive definition of the required zero test. It uses no minimization.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [12F](../../12f.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ii](../../../split.md)
5. [2021](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
