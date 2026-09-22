<h1 id="5e/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Choose a [right inverse](../../../../../../right-inverse.md) $s:A\to B$ of the [surjection](../../../../../../surjective-function.md) $f$, so $f(s(a))=a$, and define

$$
\boxed{h=g\circ s.}
$$

For each $a$, the element $b=s(a)$ then witnesses both $f(b)=a$ and $g(b)=h(a)$. As in part (a), arbitrary simultaneous choices use the [axiom of choice](../../../../../../axiom-of-choice.md). If $A$ is empty, surjectivity and the existence of $f:B\to A$ force $B$ to be empty, and the unique empty function $h:A\to C$ already meets the requirement.

Suppose $g$ is constant on each [fiber of a function](../../../../../../fiber-of-a-function.md) of $f$. Since every fiber is nonempty, $h(a)$ must be its common $g$-value: any witness $b$ in that fiber gives that value. This defines exactly one $h$ and yields $g=h\circ f$, an instance of [factorization through a surjection](../../../../../../factorization-through-a-surjection.md).

Conversely, suppose a fiber contains $b,b'$ with $f(b)=f(b')=a_0$ but $g(b)\ne g(b')$. Starting with any admissible $h$, define $h_1,h_2$ to agree with it away from $a_0$, but put $h_1(a_0)=g(b)$ and $h_2(a_0)=g(b')$. Both remain admissible, witnessed at $a_0$ by $b$ and $b'$ respectively, yet they are distinct. Hence

$$
\boxed{h\text{ is unique}\iff f(b)=f(b')\Longrightarrow g(b)=g(b').}
$$

The distinction is important: the original existence property asks only for one witness in each fiber. Only when $g$ is fiberwise constant does that property force $g=h\circ f$ for every $b$.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5E](../../5e.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ia](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
