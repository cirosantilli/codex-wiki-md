<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For finite-valued random vectors, write $p(x,y)=P(X=x,Y=y)$ and $p_Y(y)=P(Y=y)$. The [conditional entropy](../../../../../conditional-entropy.md) is the average [entropy](../../../../../information-entropy-split.md) of the posterior distributions:

$$
H(X\mid Y)=\sum_{y:p_Y(y)>0}p_Y(y)
\left[-\sum_xp(x\mid y)\log_2p(x\mid y)\right].
$$

Equivalently, $H(X\mid Y)=-\sum_{x,y:p(x,y)>0}p(x,y)\log_2p(x\mid y)$. Since $p(x,y)=p_Y(y)p(x\mid y)$, splitting the [logarithm](../../../../../logarithm.md) gives

$$
\begin{aligned}
H(X,Y)&=-\sum_{x,y}p(x,y)\log_2p_Y(y)
-\sum_{x,y}p(x,y)\log_2p(x\mid y)\\
&=\boxed{H(Y)+H(X\mid Y)}.
\end{aligned}
$$

Use the usual convention $0\log_20=0$ and omit conditionals at zero-[probability](../../../../../probability.md) outputs. The same identities hold for countable alphabets whenever the [entropy](../../../../../information-entropy-split.md) sums are well-defined, without subtracting two infinite quantities.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the communication Theory course of the University of Oxford](../../../../split.md)
6. [Communication Theory course of the University of Oxford](../../../../../communication-theory-course-of-the-university-of-oxford.md)
7. [Year 3 of the mathematics course of the University of Oxford](../../../../../year-3-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
