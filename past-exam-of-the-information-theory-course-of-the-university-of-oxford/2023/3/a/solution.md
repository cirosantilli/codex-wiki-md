<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The specified transition law is a [binary erasure channel](../../../../binary-erasure-channel.md). For an input [bit](../../../../bit.md) with $\Pr(X=1)=a$, its [Shannon entropy](../../../../information-entropy-split.md) is the [binary entropy](../../../../binary-entropy.md) $h_2(a)$. A non-erased output determines $X$, whereas the erasure symbol leaves its [probability distribution](../../../../probability-distribution-split.md) unchanged because the erasure event is [independent](../../../../independent-random-variables.md) of $X$. Thus

$$
H(X\mid Y)=qH(X),\qquad I(X;Y)=(1-q)H(X)=(1-q)h_2(a).
$$

Maximizing the [mutual information](../../../../mutual-information.md) over the input [probability distribution](../../../../probability-distribution-split.md), $h_2(a)\leq1$ with equality at $a=1/2$, gives

$$
\boxed{C=1-q\quad\text{bits per channel use}.}
$$

This includes $q=0$, a noiseless binary [channel](../../../../communication-channel.md), and $q=1$, a completely erased [channel](../../../../communication-channel.md) with zero [channel capacity](../../../../channel-capacity.md).

## ↑ Ancestors (12)

1. [A](../a.md)
2. [3](../../3.md)
3. [2023](../../../2023-split.md)
4. [Past exam of the information theory course of the University of Oxford](../../../split.md)
5. [Information theory course of the University of Oxford](../../../../information-theory-course-of-the-university-of-oxford.md)
6. [Year 3 of the mathematics course of the University of Oxford](../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
7. [Mathematics course of the University of Oxford](../../../../mathematics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
