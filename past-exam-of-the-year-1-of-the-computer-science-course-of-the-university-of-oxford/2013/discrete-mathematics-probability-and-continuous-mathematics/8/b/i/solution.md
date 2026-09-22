<h1 id="8/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

[Independence of random variables](../../../../../../independent-random-variables.md) factors the [joint probability mass function](../../../../../../joint-probability-mass-function.md) as $\mathbb P(X=x,Y=y)=\mathbb P(X=x)\mathbb P(Y=y)$. Therefore

$$
\begin{aligned}
\mathbb E[f(X)g(Y)]
&=\sum_x\sum_y f(x)g(y)\mathbb P(X=x,Y=y)\\
&=\sum_x\sum_y f(x)\mathbb P(X=x)g(y)\mathbb P(Y=y)\\
&=\left(\sum_x f(x)\mathbb P(X=x)\right)\left(\sum_y g(y)\mathbb P(Y=y)\right).
\end{aligned}
$$

With finite [expected values](../../../../../../expected-value-split.md), these rearrangements are justified by absolute convergence: the analogous sum with absolute values equals $\mathbb E[|f(X)|]\mathbb E[|g(Y)|]<\infty$. Thus

$$
\boxed{\mathbb E[f(X)g(Y)]=\mathbb E[f(X)]\mathbb E[g(Y)].}
$$

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [8](../../../8.md)
4. [Discrete mathematics, probability and continuous mathematics](../../../../discrete-mathematics-probability-and-continuous-mathematics-split.md)
5. [2013](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
