<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let the [probability](../../../../probability.md) of the first input be $t$. The two equal output probabilities are $(2+t)/6$, and the third is $s=(1-t)/3$. Writing $h_2$ for the [binary entropy function](../../../../binary-entropy-function.md), the output [entropy](../../../../information-entropy-split.md) is $h_2(s)+(1-s)$, while the [conditional entropy](../../../../conditional-entropy.md) is $t+(1-t)\log_2 3$. Therefore

$$
I(t)=h_2(s)-s\log_2(27/4),\qquad0\leq s\leq\frac13.
$$

The derivative with respect to $s$ is

$$
\log_2\frac{1-s}{s}-\log_2\frac{27}4,
$$

and the second derivative is $-1/(\ln2\,s(1-s))<0$ in the interior. Thus the unique stationary point is the global maximum. It occurs at $s=4/31$, so

$$
\boxed{P_X=(19/31,12/31)}.
$$

The capacity itself is $\boxed{C=\log_2(31/27)}$. The maximization is over $t$, not over arbitrary output distributions; $s=(1-t)/3$ keeps the feasible outputs explicit.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [3](../../3.md)
3. [2009](../../../2009-split.md)
4. [Past exam of the communication Theory course of the University of Oxford](../../../split.md)
5. [Communication Theory course of the University of Oxford](../../../../communication-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
