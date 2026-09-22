<h1 id="2/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Let $X$ be the original input, $U$ the output of the first channel, and $Y$ the final output. The [independent](../../../../../independent-random-variables.md) erasure flag is observable from $Y$. The [mutual information](../../../../../mutual-information.md) chain rule, conditioning on that flag, gives

$$
I(X;Y)=(1-\epsilon)I(X;U)+\epsilon\cdot0.
$$

The same uniform input maximizes $I(X;U)$ as in the [binary symmetric channel](../../../../../binary-symmetric-channel.md). Thus

$$
\boxed{C=(1-\epsilon)(1-h(p))}.
$$

This scaling works because the erasure event is [independent](../../../../../independent-random-variables.md) of both the input and the first channel noise.

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [2](../../../2.md)
4. [2008](../../../../2008-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
