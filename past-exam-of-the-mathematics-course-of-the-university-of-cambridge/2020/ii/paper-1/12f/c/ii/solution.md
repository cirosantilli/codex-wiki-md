<h1 id="12f/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

The function $h$ is also not partial computable. On every odd input it is defined, and

$$
h(n)=0
\quad\Longleftrightarrow\quad
f_{n,1}(n)\text{ is undefined}
\qquad(n\text{ odd}),
$$

because the value in the halting case is $f_{n,1}(n)+1\ge1$. Thus a machine computing $h$ would decide diagonal halting for odd program indices simply by running $h(n)$ and testing whether its output is zero.

That restricted problem remains undecidable. By the [padding lemma](../../../../../../../padding-lemma.md), an arbitrary machine can effectively be replaced by an equivalent machine having an odd code—for example by adding unreachable instructions until the chosen effective encoding has the required parity. This gives a computable reduction from unrestricted diagonal halting to diagonal halting on odd indices. A decider obtained from $h$ would therefore decide the full diagonal halting problem, a contradiction. Hence

$$
\boxed{h\text{ is not partial computable}}.
$$

## ↑ Ancestors (12)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [12F](../../../12f.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [Ii](../../../../split.md)
6. [2020](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
